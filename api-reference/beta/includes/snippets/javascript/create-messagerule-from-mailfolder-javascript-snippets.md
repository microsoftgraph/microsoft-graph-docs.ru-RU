---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5ff708889bdd350f070066f8dfe05f2ac504ef1e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809948"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const messageRule = {
    displayName: 'From partner',      
    sequence: 2,      
    isEnabled: true,          
    conditions: {
        senderContains: [
          'adele'       
        ]
     },
     actions: {
        forwardTo: [
          {
             emailAddress: {
                name: 'Alex Wilbur',
                address: 'AlexW@contoso.onmicrosoft.com'
              }
           }
        ],
        stopProcessingRules: true
     }    
};

await client.api('/me/mailFolders/inbox/messagerules')
    .version('beta')
    .post(messageRule);

```