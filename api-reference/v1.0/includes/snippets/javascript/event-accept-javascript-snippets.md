---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 901d71545e8156cde08a1481f6950997a15daebd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35515985"
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
    .post(accept);

```