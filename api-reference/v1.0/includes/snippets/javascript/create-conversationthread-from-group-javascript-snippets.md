---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1309aba429eb62630eb1bd7cadcb9ac3e661a6d5289d5ec8b832d22a2c2aa27e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57152951"
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
    .post(conversationThread);

```