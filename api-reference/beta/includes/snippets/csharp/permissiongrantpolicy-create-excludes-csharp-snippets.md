---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 64f1f226892eb46fde53aec664dbfd29c9e50a55
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785871"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantConditionSet = new PermissionGrantConditionSet
{
    PermissionType = PermissionType.Delegated,
    ResourceApplication = "00000003-0000-0000-c000-000000000000"
};

await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"].Excludes
    .Request()
    .AddAsync(permissionGrantConditionSet);

```