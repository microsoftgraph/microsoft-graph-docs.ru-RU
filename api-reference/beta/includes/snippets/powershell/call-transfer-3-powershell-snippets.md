---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cf85e5eeec209ae54c7bdbc30970852cbed6cb86
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341402"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    TransferTarget = @{
        EndpointType = "default"
        Identity = @{
            Phone = @{
                "@odata.type" = "#microsoft.graph.identity"
                Id = "+12345678901"
            }
        }
        LanguageId = "languageId-value"
        Region = "region-value"
    }
}

Move-MgCommunicationCall -CallId $callId -BodyParameter $params

```