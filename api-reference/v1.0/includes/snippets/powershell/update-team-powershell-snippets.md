---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d66fe76ef5f75cb62efddd6015f3f56aace639d7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128357"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    MemberSettings = @{
        AllowCreateUpdateChannels = $true
    }
    MessagingSettings = @{
        AllowUserEditMessages = $true
        AllowUserDeleteMessages = $true
    }
    FunSettings = @{
        AllowGiphy = $true
        GiphyContentRating = "strict"
    }
}

Update-MgTeam -TeamId $teamId -BodyParameter $params

```