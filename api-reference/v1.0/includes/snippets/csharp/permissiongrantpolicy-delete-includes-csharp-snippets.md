---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 20e869a9bce15bb70499e20445a3da54e0a95443
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796399"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"].Includes["{permissionGrantConditionSet-id}"]
    .Request()
    .DeleteAsync();

```