---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 87f310a85515e7b6d505c77429e9f5894a4d8f01
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205401"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleAssignmentSchedule = await client.api('/roleManagement/directory/roleAssignmentSchedules/95c690fb-3eb3-4942-a03f-4524aed6f31e')
    .get();

```