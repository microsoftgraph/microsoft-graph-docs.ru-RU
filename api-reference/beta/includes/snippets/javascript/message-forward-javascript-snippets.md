---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff47ebac31ccbcd132bafb64dcece94bd724edae
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35489118"
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