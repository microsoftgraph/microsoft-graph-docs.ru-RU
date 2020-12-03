---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2239dcce419b9c3e296454d5d476fd65f57b3e20
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantPolicies = await graphClient.Policies.PermissionGrantPolicies
    .Request()
    .GetAsync();

```