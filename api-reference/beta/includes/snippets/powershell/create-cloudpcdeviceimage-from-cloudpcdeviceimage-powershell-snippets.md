---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 745149cd4b03a49537835e65c586f09dce5d67da
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122541"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

$params = @{
    "@odata.type" = "#microsoft.graph.cloudPcDeviceImage"
    DisplayName = "Display Name value"
    OsBuildNumber = "OS Build Number value"
    OperatingSystem = "Operating System value"
    Version = "Version value"
    SourceImageResourceId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage"
}

New-MgDeviceManagementVirtualEndpointDeviceImage -BodyParameter $params

```