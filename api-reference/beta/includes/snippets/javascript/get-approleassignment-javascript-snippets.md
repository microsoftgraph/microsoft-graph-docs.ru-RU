---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 248228537a7aa1946e553fc0a641d8a5b8057364
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529899"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appRoleAssignments/{id}')
    .version('beta')
    .get();

```