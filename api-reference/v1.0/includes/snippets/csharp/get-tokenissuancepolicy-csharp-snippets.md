---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a79d3534fc09bfafbf25f7f34ff5d3d35a56ba1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807928"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicy = await graphClient.Policies.TokenIssuancePolicies["{tokenIssuancePolicy-id}"]
    .Request()
    .GetAsync();

```