---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 71383ac790f1d1ef228249a1ddd563f141b7ea31265d0173b789fdb2ccd76eba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57140016"
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
    .version('beta')
    .post(conversationThread);

```