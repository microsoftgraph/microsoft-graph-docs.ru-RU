---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8aea18bb41934dc4eea9142b60f4d192565a454b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133579"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    OriginalStartTimeZone = "originalStartTimeZone-value"
    OriginalEndTimeZone = "originalEndTimeZone-value"
    ResponseStatus = @{
        Response = ""
        Time = [System.DateTime]::Parse("datetime-value")
    }
    Uid = "iCalUId-value"
    ReminderMinutesBeforeStart = 99
    IsReminderOn = $true
}

Update-MgGroupEvent -GroupId $groupId -EventId $eventId -BodyParameter $params

```