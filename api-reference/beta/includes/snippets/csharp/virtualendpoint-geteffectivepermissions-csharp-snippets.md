---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 44f0a918300ca0beed076e825b1aca4204d0e03b
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522337"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEffectivePermissions = await graphClient.DeviceManagement.VirtualEndpoint
    .GetEffectivePermissions()
    .Request()
    .GetAsync();

```