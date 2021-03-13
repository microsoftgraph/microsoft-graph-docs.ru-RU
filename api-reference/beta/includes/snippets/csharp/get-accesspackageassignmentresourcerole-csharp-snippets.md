---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 16ef993dd9d29ce04484f4482a5c4bd8e69d15c5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778427"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignmentResourceRole = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentResourceRoles["{accessPackageAssignmentResourceRole-id}"]
    .Request()
    .GetAsync();

```