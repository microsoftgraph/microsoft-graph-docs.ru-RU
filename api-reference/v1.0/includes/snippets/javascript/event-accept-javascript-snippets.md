---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 15e0267f029a3e4129fe45cceea9a9dc2284af74
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785240"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accept = {
  comment: 'comment-value',
  sendResponse: true
};

await client.api('/me/events/{id}/accept')
    .post(accept);

```