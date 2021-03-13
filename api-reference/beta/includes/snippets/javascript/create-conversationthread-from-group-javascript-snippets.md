---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2978b5cbb0d0f68cecd30b47ee1e066efe9b8f26
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785412"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  topic: 'New Conversation Thread Topic',
  posts: [{
    body: {
      contentType: 'html',
      content: 'this is body content'
    },
    newParticipants: [{
      emailAddress: {
        name: 'Alex Darrow',
        address: 'alexd@contoso.com'
      }
    }]
  }]
};

await client.api('/groups/{id}/threads')
    .version('beta')
    .post(conversationThread);

```