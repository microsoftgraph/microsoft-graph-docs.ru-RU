---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6ea2589847869b8034246e47e8eedb8f2beb2d1e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720315"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedApproval = {
  userId: "userId-value",
  roleId: "roleId-value",
  approvalType: "approvalType-value",
  approvalState: "approvalState-value",
  approvalDuration: "datetime-value"
};

let res = await client.api('/privilegedApproval')
    .version('beta')
    .post({privilegedApproval : privilegedApproval});

```