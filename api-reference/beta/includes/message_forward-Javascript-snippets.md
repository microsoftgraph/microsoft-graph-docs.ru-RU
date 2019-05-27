---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff47ebac31ccbcd132bafb64dcece94bd724edae
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444015"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forward = {
  message:{  
    isDeliveryReceiptRequested: true,
    toRecipients:[
      {
        emailAddress: {
          address:"danas@contoso.onmicrosoft.com",
          name:"Dana Swope"
        }
      }
     ]
  },
  comment: "Dana, just want to make sure you get this." 
};

let res = await client.api('/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward')
    .version('beta')
    .post(forward);

```