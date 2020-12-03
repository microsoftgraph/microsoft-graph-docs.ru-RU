---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 689664cef43173dfad8793ba83183b802d298629
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521434"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcProvisioningPolicy = new CloudPcProvisioningPolicy
{
    DisplayName = "Display Name value",
    Description = "Description value",
    OnPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
    ImageId = "Image ID value",
    ImageDisplayName = "Image Display Name value",
    ImageType = CloudPcProvisioningPolicyImageType.Custom
};

await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies["{id}"]
    .Request()
    .UpdateAsync(cloudPcProvisioningPolicy);

```