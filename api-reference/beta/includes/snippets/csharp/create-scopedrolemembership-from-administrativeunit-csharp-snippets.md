---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3be5b5677490a14202622ef8e99c2d32395bfd82
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794938"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var scopedRoleMembership = new ScopedRoleMembership
{
    RoleId = "roleId-value",
    RoleMemberInfo = new Identity
    {
        Id = "id-value"
    }
};

await graphClient.AdministrativeUnits["{administrativeUnit-id}"].ScopedRoleMembers
    .Request()
    .AddAsync(scopedRoleMembership);

```