---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 73bfcd4185d7d8447b3642cc664dd576f3b875b1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62087724"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "Template@odata.bind" = "https://graph.microsoft.com/v1.0/teamsTemplates('standard')"
    "Group@odata.bind" = "https://graph.microsoft.com/v1.0/groups('dbd8de4f-5d47-48da-87f1-594bed003375')"
    Channels = @(
        @{
            DisplayName = "Class Announcements 📢"
            IsFavoriteByDefault = $true
        }
        @{
            DisplayName = "Homework 🏋️"
            IsFavoriteByDefault = $true
        }
    )
    MemberSettings = @{
        AllowCreateUpdateChannels = $false
        AllowDeleteChannels = $false
        AllowAddRemoveApps = $false
        AllowCreateUpdateRemoveTabs = $false
        AllowCreateUpdateRemoveConnectors = $false
    }
    InstalledApps = @(
        @{
            "TeamsApp@odata.bind" = "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"
        }
        @{
            "TeamsApp@odata.bind" = "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"
        }
    )
}

New-MgTeam -BodyParameter $params

```