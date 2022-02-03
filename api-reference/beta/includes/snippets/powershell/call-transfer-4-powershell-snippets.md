---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b290004e023ae592b8d86624b32ca134e5a076ae
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341390"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    TransferTarget = @{
        "@odata.type" = "#microsoft.graph.invitationParticipantInfo"
        EndpointType = "default"
        Identity = @{
            "@odata.type" = "#microsoft.graph.identitySet"
            Phone = @{
                "@odata.type" = "#microsoft.graph.identity"
                Id = "+12345678901"
            }
        }
        LanguageId = "en-us"
        Region = "amer"
        ReplacesCallId = "e5d39592-99bd-4db8-bca8-30fb894ec51d"
    }
}

Move-MgCommunicationCall -CallId $callId -BodyParameter $params

```