---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4e1c736346a4c55371bafd5da0cc461275efb221
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352271"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Subject = "Let's go for lunch"
    Body = @{
        ContentType = "HTML"
        Content = "Does noon work for you?"
    }
    Start = @{
        DateTime = "2017-04-15T12:00:00"
        TimeZone = "Pacific Standard Time"
    }
    End = @{
        DateTime = "2017-04-15T14:00:00"
        TimeZone = "Pacific Standard Time"
    }
    Location = @{
        DisplayName = "Harry's Bar"
    }
    Attendees = @(
        @{
            EmailAddress = @{
                Address = "samanthab@contoso.onmicrosoft.com"
                Name = "Samantha Booth"
            }
            Type = "required"
        }
    )
    AllowNewTimeProposals = $true
    IsOnlineMeeting = $true
    OnlineMeetingProvider = "teamsForBusiness"
}

# A UPN can also be used as -UserId.
New-MgUserEvent -UserId $userId -BodyParameter $params

```