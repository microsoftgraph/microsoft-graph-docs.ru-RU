---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fcb601a6db964455e96ed3233375aec49cab7bc3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616041"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteOperation = {
  id: "id-value",
  groupId: "groupId-value",
  renameAs: "renameAs-value"
};

let res = await client.api('/me/onenote/sections/{id}/copyToSectionGroup')
    .version('beta')
    .post(onenoteOperation);

```