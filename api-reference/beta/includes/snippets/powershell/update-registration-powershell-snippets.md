---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a18084ad7164634743c8ab0f52b6eb3ad609881a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113175"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    Subject = "Microsoft Ignite: Day 1"
    StartDateTime = [System.DateTime]::Parse("2021-11-02T08:00:00-08:00")
    EndDateTime = [System.DateTime]::Parse("2021-11-02T15:45:00-08:00")
    Speakers = @(
        @{
            DisplayName = "Henry Ross"
            Bio = "Chairman and Chief Executive Officer"
        }
        @{
            DisplayName = "Fred Ryan"
            Bio = "CVP"
        }
    )
}

Update-MgUserOnlineMeetingRegistration -UserId $userId -OnlineMeetingId $onlineMeetingId -BodyParameter $params

```