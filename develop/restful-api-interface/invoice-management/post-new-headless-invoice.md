---
description: Generate new payment method
---

# \[POST] New headless invoice

## Base url :&#x20;

```
/invoice/new/headless
```

## Method :&#x20;

```
POST
```

## Auth :&#x20;

```
Require
```

## Params :&#x20;

```
NONE
```

## Body  :&#x20;

<table><thead><tr><th width="288">Key</th><th>Type</th><th>Data</th></tr></thead><tbody><tr><td>amountToken</td><td>uint</td><td>amount , in token</td></tr><tr><td>amountUsd</td><td>uint</td><td>amount , in usd</td></tr><tr><td>comment</td><td>string</td><td>Some words in invoice</td></tr><tr><td>callback</td><td>string</td><td>Callback path</td></tr><tr><td>type</td><td>int</td><td>ChainId of invoice</td></tr><tr><td>token</td><td>int</td><td>TokenId of invoice</td></tr><tr><td>address</td><td>string</td><td>Reciver address</td></tr><tr><td>label</td><td>string</td><td>Invoice tittle</td></tr><tr><td>timeout</td><td>uint</td><td>Timeout limit to this invoice</td></tr></tbody></table>

## Response :&#x20;

````json
```json
{
    "code": 200, //Status code . 200 success 500 error
    "data": {
        "invoiceId": "9936ace52b30d567d55253c4a57fad8f",
        "botLink": "https://t.me/tonspay_bot?start=19936ace52b30d567d55253c4a57fad8f",
        "webLink": "https://wallet.tonspay.top/page-invoices?id=9936ace52b30d567d55253c4a57fad8f",
        "webappLink": "https://t.me/tonspay_bot/invoice?startapp=9936ace52b30d567d55253c4a57fad8f"
    }
}
```
````
