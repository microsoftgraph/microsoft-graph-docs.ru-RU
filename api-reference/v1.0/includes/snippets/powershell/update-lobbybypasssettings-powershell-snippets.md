---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 570e40d9d82aa528718b5930acc930cd957313c3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352200"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    LobbyBypassSettings = @{
        IsDialInBypassEnabled = $true
    }
}

# A UPN can also be used as -UserId.
Update-MgUserOnlineMeeting -UserId $userId -OnlineMeetingId $onlineMeetingId -BodyParameter $params

```