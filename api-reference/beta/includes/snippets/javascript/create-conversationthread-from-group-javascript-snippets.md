---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5174e7fd1e3ee28a70f272c1ff8a7af21846307d1b9fe2ec71cde94cf94feaf7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57203023"
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