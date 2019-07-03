---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0582e0d132931805a3ce3a5e0e0c9e65267f1fe2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35505864"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  comment: "comment-value",
  sendResponse: true
};

let res = await client.api('/me/events/{id}/decline')
    .version('beta')
    .post(decline);

```