---
description: >-
  Tonspay is a crypto payment solution base on Telegram-bot & webapp , support
  annoymouse payment without KYC.
---

# 😇 Welcome

### What is Tonspay

Tonspay is a crypto payment solution base on **Telegram-bot & webapp** , support annoymouse payment **without KYC**.

Tonspay supporty for multichains payment , including : **TON** | **SOLANA** | **ARBITRUM** | **TRON** and **Binance-pay** . It provide a fully document restful-api and callback system for any merchant to onboard easily . The merchant of Tonspay can manage it's invoices by using **Tonspay-bot** | **Restful-api** | **Tonspay-dashboard** .&#x20;

Tonspay also working on low-code onboarding , Which should help those un-dev merchant to build it's own telegram-bot online shop using Tonspay as crypto payment solution.

### Why Tonspay&#x20;

Telegram-bot & Telegram-webapp needs a stable and easy use invoice-base cypto payment system . Anyone can use Tonspay to generate a invoice for crypto payment , and the fund will directly send to merchant's crypto account . No need any KYC .

### How Tonspay work

<figure><img src=".gitbook/assets/Tonspay.png" alt=""><figcaption><p>How Tonspay work</p></figcaption></figure>

### Tonspay open source ?&#x20;

#### Currently tonspay are opensource parts :&#x20;

* [Tonspay-onchain-monitor](https://github.com/Tonspay/Tonspay-monitor)
* [Tonspay-evm-chain-payment-contract](https://github.com/Tonspay/Tonspay-evm-router-contract)
* [Tonspay-demo-merchant-bot](https://github.com/Tonspay/Tonspay-demo-steam-mystery-box-bot)
* [Tonspay-main-websit](https://github.com/Tonspay/Tonspay-websit)

#### As for the paymenst service-backend is not opensource yet.But it will publish it's framwork :

* #### Tonspay Server
  * Restful Interface
    * New Invoice
    * Invoice Status
    * Invoice Callback
  * Web Interface
    * Account managment
    * Account payment method
      * Ln
      * Evm
      * Ton
      * Tron
* #### Tonspay Bot
  * Account management
  * Account payment method
  * Bot payment management
  * Invoice management
    * Invoice generate
    * Invoice status check
    * Invoice callback to bot
  * Payment action
    * Payment action
    * Payment callback
* Tonspay webapp
  * User wallet management  & connection
  * User invoices & actives managment
  * Payment actions
    * Pay invoices
    * Cancel invoices
  * Cash gift actions
    * Gnerate a new cash gift
    * Deposit money into it&#x20;
