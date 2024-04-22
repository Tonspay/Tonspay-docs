---
description: The callback body sign and verfiy logic .
---

# Callback ${body}

The callback body will be sign by a keypair of Tonspay official to avoid callback interface being witch attack .

**Body** :

```json
{
    sign : "The signature data to prove message sended from tonspay"
}
```

The `sign` are a signature that using `ed25519` . Result being encode by `base58` , please decode it into bytes by base58.

You will be able to deocde the signature-data by `tweetnacl` into data `${base64-data}`.

**Base64-data** decode with `json.parse`:

```json
{
           "uid":0, //Your merchant user id in telegram bot . Please verfiy if it is your callback.
            "invoiceId":"",//Which invoice this callback for . 
            "paymentMethod":"",//The payment method of the invoice . 
            "confirmedBlock":"", //How many block since the callback confirm . 
            "paymentDetails":{
                    "from":"",//The address of payer . 
                    "amount":0,//How much this transaction paid on chain .
                    "hash" : "",//The transaction hash of this payment . 
            },
            "routerFeeDetails":{
                    "from":"",//The address of payer . 
                    "amount":"",//How much being charged by payment router .
                    "hash" : "" , //The sub transaction of router fee .
                    "isPrepaid":bool, //If this transaction being prepaird by merchant by Token . 
            },
            "createTime":0//The time of this callback .
},
```

Tonspay signature **publick-key**&#x20;

**Production ENV :**

```
ENzsJ58Lmb6GMfMPhsTKm1AYaEoL5Z24r9RVPKaYLyJ6
```

**Test/Sandbox  ENV :** &#x20;

```
2885LXvdSb9FYxrr8BD5tgML3hXdWbC33ofT3MWqhZtQ
```

**Verfiy logic in js** :

```javascript
const signData = b58.decode(rawData.sign);

const decodeData = nacl.sign.open( signData, b58.decode('ENzsJ58Lmb6GMfMPhsTKm1AYaEoL5Z24r9RVPKaYLyJ6'))

const finalData = json.parse(
    Buffer.from(decodeData).toString()
)
```
