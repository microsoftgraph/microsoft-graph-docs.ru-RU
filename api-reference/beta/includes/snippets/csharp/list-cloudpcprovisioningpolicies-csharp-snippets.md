---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7a3a4b3d3033e10467a62a8736b5564b9502997b
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522590"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var provisioningPolicies = await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies
    .Request()
    .GetAsync();

```