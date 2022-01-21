---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: abeb99f7cd0f771ec33ec5f8afb14ddb72de51c0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134958"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Body = @{
        ContentType = "html"
        Content = "Hello World"
    }
}

New-MgTeamChannelMessageReply -TeamId $teamId -ChannelId $channelId -ChatMessageId $chatMessageId -BodyParameter $params

```