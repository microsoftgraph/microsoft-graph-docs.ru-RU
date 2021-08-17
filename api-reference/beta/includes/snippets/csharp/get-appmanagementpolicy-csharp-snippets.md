---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1dc7907e52b9c03231db5a71869d672b7d9a3ce0
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259041"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appManagementPolicy = await graphClient.Policies.AppManagementPolicies["{appManagementPolicy-id}"]
    .Request()
    .GetAsync();

```