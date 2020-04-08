---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 993eaff233589c8791a0bb52dc1cf68fd481f02a
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181171"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignment = new UnifiedRoleAssignment
{
    RoleDefinitionId = "fe930be7-5e62-47db-91af-98c3a49a38b1",
    PrincipalId = "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    DirectoryScopeId = "5d107bba-d8e2-4e13-b6ae-884be90e5d1a"
};

await graphClient.RoleManagement.Directory.RoleAssignments
    .Request()
    .AddAsync(unifiedRoleAssignment);

```