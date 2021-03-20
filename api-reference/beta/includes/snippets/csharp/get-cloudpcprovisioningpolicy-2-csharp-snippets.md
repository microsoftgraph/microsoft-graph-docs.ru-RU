---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6d031f3da9b190a9546bc52e31185b762ba6451b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947575"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcProvisioningPolicy = await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies["{cloudPcProvisioningPolicy-id}"]
    .Request()
    .Expand("assignments")
    .GetAsync();

```