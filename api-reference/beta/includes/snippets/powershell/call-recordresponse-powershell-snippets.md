---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3a10772fe6e1f5d3381dedd8ffb53f77ecccdc7e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346968"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    BargeInAllowed = $true
    ClientContext = "d45324c1-fcb5-430a-902c-f20af696537c"
    Prompts = @(
        @{
            "@odata.type" = "#microsoft.graph.mediaPrompt"
        }
    )
    MaxRecordDurationInSeconds = 10
    InitialSilenceTimeoutInSeconds = 5
    MaxSilenceTimeoutInSeconds = 2
    PlayBeep = $true
    StopTones = @(
        "#"
        "1"
        "*"
    )
}

Invoke-MgRecordCommunicationCallResponse -CallId $callId -BodyParameter $params

```