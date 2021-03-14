---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b1308d0039fc8d856f16b39e96bd9ae3f514b7fc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791641"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  topic: 'topic-value',
  posts: [{
      body: {
        contentType: 'html',
        content: 'this is body content'
      }
  }]
};

await client.api('/groups/{id}/conversations/{id}/threads')
    .post(conversationThread);

```