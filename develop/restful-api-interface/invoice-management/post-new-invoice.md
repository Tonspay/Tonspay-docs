---
description: Generate new payment method
---

# \[POST] New invoice

## Base url :&#x20;

```
/invoice/new
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

<table><thead><tr><th width="288">Key</th><th>Type</th><th>Data</th></tr></thead><tbody><tr><td>amountToken</td><td>uint</td><td>amount , in token</td></tr><tr><td>amountUsd</td><td>uint</td><td>amount , in usd</td></tr><tr><td>paymentMethodId</td><td>string</td><td>Id of using payment method</td></tr><tr><td>comment</td><td>string</td><td>Some words in invoice</td></tr><tr><td>callback</td><td>string</td><td>Callback path</td></tr></tbody></table>

