---
description: Crosschain payment of Tonspay
---

# Crosschain Payment

By supporting [Wallet-V5](https://github.com/tonkeeper/w5) & [FixFloat](https://ff.io/), Tonspay can paid transactions for users . Which means Tonspay support crosschain payment & transactions .&#x20;

For example . User A have TON wallet `ton_A` , but it have no TON . Then User A wants to purchas token `token_a` on TON . By using Tonspay , User A can sign a purchas singature via `ton_A` , and Tonspay will generate an invoice for this action , allows user to paied via differents chain including Solana / Arbitrum / Binance Pay . All the paymen will directly bridge to `ton_A` using FixFloat, and when the bridge success , Tonspay will auto boardcast transaction that signed before on TON .

## How crosschian payment works ?

For crosschain payment , generally can splited into few step :&#x20;

1. Gnerate pre-payment signature & hash , and signed by User .&#x20;
2. Bridge the asserts through FixFloat .&#x20;
3. When brdige callback , Send signed transaction on chain .&#x20;

All step are safe and decentralized . It will no more require user to have TON coin for start a new payment . Tonspay can help user to send out the payment via crosschain .
