---
description: Generate new payment method
---

# \[POST] New payment method

## Base url :&#x20;

```
/setting/paymentmethod/new
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

<table><thead><tr><th width="288">Key</th><th>Type</th><th>Data</th></tr></thead><tbody><tr><td>type</td><td>uint</td><td>The payment chain type</td></tr><tr><td>token</td><td>uint</td><td>The payment token type</td></tr><tr><td>address</td><td>string</td><td>The reciver address</td></tr><tr><td>callback</td><td>string</td><td>Default callback path</td></tr><tr><td>lable</td><td>string</td><td>Default payment lable</td></tr></tbody></table>

