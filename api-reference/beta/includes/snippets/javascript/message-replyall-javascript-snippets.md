---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9b9b917972b8534d95066ec5c297d5e3dfb14436
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792976"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const replyAll = {
    message: {
      attachments: [ 
        { 
          '@odata.type': '#microsoft.graph.fileAttachment', 
          name: 'guidelines.txt', 
          contentBytes: 'bWFjIGFuZCBjaGVlc2UgdG9kYXk=' 
        } 
      ]
    },
    comment: 'Please take a look at the attached guidelines before you decide on the name.' 
};

await client.api('/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll')
    .version('beta')
    .post(replyAll);

```