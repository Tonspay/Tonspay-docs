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

**Base url**

```
https://api.tonspay.top/
```

**Authenticator**

* Step 1 : Generate your _merchant-api-key_ via [telegram bot](https://t.me/tonspay\_bot?start=keygen)
* Step 2 : Set request header&#x20;

| Header | Data               |
| ------ | ------------------ |
| token  | _merchant-api-key_ |

