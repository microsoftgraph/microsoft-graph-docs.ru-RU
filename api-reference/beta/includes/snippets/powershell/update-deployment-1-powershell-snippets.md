---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 35c84bc9752f2685f4a58eea7ea765a587edd9b0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095626"
---
```powershell

Import-Module Microsoft.Graph.WindowsUpdates

$params = @{
    "@odata.type" = "#microsoft.graph.windowsUpdates.deployment"
    State = @{
        "@odata.type" = "microsoft.graph.windowsUpdates.deploymentState"
        RequestedValue = "paused"
    }
}

Update-MgWindowsUpdatesDeployment -DeploymentId $deploymentId -BodyParameter $params

```