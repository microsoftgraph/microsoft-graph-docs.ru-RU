---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 97b80561770acfde66f61a04ec266948ed29bc54
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607960"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleAssignment = new PrivilegedRoleAssignment
{
    UserId = "userId-value",
    RoleId = "roleId-value"
};

await graphClient.PrivilegedRoleAssignments
    .Request()
    .AddAsync(privilegedRoleAssignment);

```