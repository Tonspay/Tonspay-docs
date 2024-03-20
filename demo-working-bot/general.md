---
description: A working demo using tonspay as merchant system for Steam CD key selling .
---

# General

## Steam Mystery Boxes Bot

[@Steam\_mystery\_boxes\_bot](https://t.me/Steam\_mystery\_boxes\_bot) is a bot for selling Steam-mystery-CD-key . It allows user to buy random CD-key of **SteamGame** . Anyone can purchas it using crypto currency by **Tonspay .**

### Logic map

The **Steam Mystery Boxes Bot** (name it bot ) working with follow logic &#x20;

* User select a payment method , and set-up order to purchas a box .
* Bot generate a invoice & match a cd-key .&#x20;
* Bot back-end send request to Tonspay-api with `merchant-api-key` to generate payment invoice .
* Bot send payment invoice to user .
* User pay the invoice or share the invoice to others to pay .
* Tonspay server callback request Bot back-end .
* Bot back-end send the Steam CD Key to User . Invoice finished.

### More informations&#x20;

[Source code](https://github.com/Tonspay/Tonspay-demo-steam-mystery-box-bot)
