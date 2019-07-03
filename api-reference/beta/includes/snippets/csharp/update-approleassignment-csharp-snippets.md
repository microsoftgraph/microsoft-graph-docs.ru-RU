---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c17e63f645ee85200cd271bb8694f830d154decc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35505835"
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

await graphClient.AppRoleAssignments["{id}"]
    .Request()
    .UpdateAsync(appRoleAssignment);

```