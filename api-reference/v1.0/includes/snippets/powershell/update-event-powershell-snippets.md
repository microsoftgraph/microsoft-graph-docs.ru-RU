---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fd3b72c3211d3e1e738f4f948f150d5af5da4e2c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350869"
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
    Recurrence = $null
    ReminderMinutesBeforeStart = 99
    IsOnlineMeeting = $true
    OnlineMeetingProvider = "teamsForBusiness"
    IsReminderOn = $true
    HideAttendees = $false
    Categories = @(
        "Red category"
    )
}

# A UPN can also be used as -UserId.
Update-MgUserEvent -UserId $userId -EventId $eventId -BodyParameter $params

```