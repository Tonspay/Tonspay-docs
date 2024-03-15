---
description: The websocket interface of payment callback
---

# Websocket interface



*   Pre-listen subscript request :

    * Send in json

    ```json
    {
       "action" : "subscript",
       "merchanKey":"Your-merchant-api-kay" 
    }
    ```
* Payment callback :
  * Recive in json : `${body}`
