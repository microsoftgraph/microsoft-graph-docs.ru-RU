---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1cee33b7966fa42ac4faf4e78c7f2470c466e791
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124959"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "@odata.type" = "#microsoft.graph.aadUserConversationMember"
    Roles = @(
        "owner"
    )
    "User@odata.bind" = "https://graph.microsoft.com/v1.0/users('jacob@contoso.com')"
}

New-MgTeamChannelMember -TeamId $teamId -ChannelId $channelId -BodyParameter $params

```