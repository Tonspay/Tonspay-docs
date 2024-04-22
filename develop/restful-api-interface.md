---
description: The restfil api system of tonspay
---

# 🎓 Restful Api Interface

### **What can restful api do ?**

**The restful api interface will provide functions for merchant to :**

* Manage payment method
  * New payment method
  * Del payment method
* Mange invoices
  * Invoices generator
  * Invoices close
  * Invoices callback
* Manage cash-gift
  * Cashgift generator

### Base informations&#x20;

**Production Base url**

```
https://api.tonspay.top/
```

```
https://wallet.tonspay.top/api
```

#### **Testnet Base url**

```
https://test.tonspay.top/api
```

```
https://test-api.tonspay.top/
```

**Authenticator**

* Step 1 : Generate your _merchant-api-key_ via [telegram bot](https://t.me/tonspay\_bot?start=keygen)
* Step 2 : Set request header&#x20;

| Header | Data               |
| ------ | ------------------ |
| token  | _merchant-api-key_ |

