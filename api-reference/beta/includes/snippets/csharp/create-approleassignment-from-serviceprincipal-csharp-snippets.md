---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8e1ef2af7a58386f36f4233796be08590968a384
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35528194"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appRoleAssignment = new AppRoleAssignment
{
    CreationTimestamp = "2016-10-19T10:37:00Z",
    PrincipalDisplayName = "principalDisplayName-value",
    PrincipalId = "principalId-value",
    PrincipalType = "principalType-value",
    ResourceDisplayName = "resourceDisplayName-value"
};

await graphClient.ServicePrincipals["{id}"].AppRoleAssignments
    .Request()
    .AddAsync(appRoleAssignment);

```