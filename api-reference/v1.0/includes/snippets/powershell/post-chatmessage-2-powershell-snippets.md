---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0b3b16e4deaca9c61765fda18aa8016a8f2bf047
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129131"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Body = @{
        ContentType = "html"
        Content = "Hello World <at id="0">Jane Smith</at>"
    }
    Mentions = @(
        @{
            Id = 0
            MentionText = "Jane Smith"
            Mentioned = @{
                User = @{
                    DisplayName = "Jane Smith"
                    Id = "ef1c916a-3135-4417-ba27-8eb7bd084193"
                    UserIdentityType = "aadUser"
                }
            }
        }
    )
}

New-MgTeamChannelMessage -TeamId $teamId -ChannelId $channelId -BodyParameter $params

```