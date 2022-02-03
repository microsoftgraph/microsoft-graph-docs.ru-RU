---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2b0a06c30903c24a4f32577d9e225643e9c37f5d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341953"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    AtAprovedLocation = $true
    Notes = @{
        ContentType = "text"
        Content = "start break smaple notes"
    }
}

Start-MgTeamScheduleTimeCardBreak -TeamId $teamId -TimeCardId $timeCardId -BodyParameter $params

```