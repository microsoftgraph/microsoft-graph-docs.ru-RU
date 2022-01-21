---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0d231341e827e4f17855290091abcf2c9332ebc5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126824"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    IsMembershipLimitedToOwners = $true
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
    DiscoverySettings = @{
        ShowInTeamsSearchAndSuggestions = $true
    }
}

Update-MgTeam -TeamId $teamId -BodyParameter $params

```