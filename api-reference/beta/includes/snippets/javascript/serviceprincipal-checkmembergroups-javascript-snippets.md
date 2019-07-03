---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 19a6ba5fb1a41f1b0a5fa37315caf50cdcc83e04
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35489548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const String = {
  groupIds: [
    "groupIds-value"
  ]
};

let res = await client.api('/servicePrincipals/{id}/checkMemberGroups')
    .version('beta')
    .post(String);

```