---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 875d6224d46f1326089b168c3845f4f516771873
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800385"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const replyAll = {
  comment: 'comment-value'
};

await client.api('/me/messages/{id}/replyAll')
    .post(replyAll);

```