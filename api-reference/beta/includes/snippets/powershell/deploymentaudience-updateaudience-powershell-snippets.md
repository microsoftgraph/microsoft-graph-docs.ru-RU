---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 427680553ab3cb1df7b0c776bee2758d79ec79d4
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348163"
---
```powershell

Import-Module Microsoft.Graph.WindowsUpdates

$params = @{
    AddMembers = @(
        @{
            "@odata.type" = "#microsoft.graph.windowsUpdates.updatableAsset"
            Id = "String (identifier)"
        }
    )
    RemoveMembers = @(
        @{
            "@odata.type" = "#microsoft.graph.windowsUpdates.updatableAsset"
            Id = "String (identifier)"
        }
    )
    AddExclusions = @(
        @{
            "@odata.type" = "#microsoft.graph.windowsUpdates.updatableAsset"
            Id = "String (identifier)"
        }
    )
    RemoveExclusions = @(
        @{
            "@odata.type" = "#microsoft.graph.windowsUpdates.updatableAsset"
            Id = "String (identifier)"
        }
    )
}

Update-MgWindowsUpdatesDeploymentAudience -DeploymentId $deploymentId -BodyParameter $params

```