---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2efcf1110ff826e31bae89e5058f1bcc9eba78cd
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347837"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    ClientContext = "d45324c1-fcb5-430a-902c-f20af696537c"
    Prompts = @(
        @{
            "@odata.type" = "#microsoft.graph.mediaPrompt"
            MediaInfo = @{
                "@odata.type" = "#microsoft.graph.mediaInfo"
                Uri = "https://cdn.contoso.com/beep.wav"
                ResourceId = "1D6DE2D4-CD51-4309-8DAA-70768651088E"
            }
        }
    )
}

Invoke-MgPlayCommunicationCallPrompt -CallId $callId -BodyParameter $params

```