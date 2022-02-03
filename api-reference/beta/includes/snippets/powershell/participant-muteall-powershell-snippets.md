---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 227b52cb0974d426964ebba2973579976b270252
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341994"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    Participants = @(
        ""
    )
    ClientContext = "clientContext-value"
}

Invoke-MgMuteCommunicationCallParticipant -CallId $callId -BodyParameter $params

```