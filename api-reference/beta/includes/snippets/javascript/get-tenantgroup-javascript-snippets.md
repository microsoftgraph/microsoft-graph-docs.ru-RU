---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 064ce64edaa71237c4f92326ff807ee2da7f7bfc
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441167"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenantGroup = await client.api('/tenantRelationships/managedTenants/tenantGroups/{tenantGroupId}')
    .version('beta')
    .get();

```