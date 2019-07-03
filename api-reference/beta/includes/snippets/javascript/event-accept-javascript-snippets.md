---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8c6ae08e66e0420b5226a83f6224513e118c3aed
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35505871"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accept = {
  comment: "comment-value",
  sendResponse: true
};

let res = await client.api('/me/events/{id}/accept')
    .version('beta')
    .post(accept);

```