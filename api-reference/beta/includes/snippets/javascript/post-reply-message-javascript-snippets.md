---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9ad3ab7e56aff5b4fb1ebd14964f686b9db647b6
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638250"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  body: {
    contentType: "html",
    content: "Hello World"
  }
};

let res = await client.api('/teams/{id}/channels/{id}/messages/{id}/replies')
    .version('beta')
    .post(chatMessage);

```