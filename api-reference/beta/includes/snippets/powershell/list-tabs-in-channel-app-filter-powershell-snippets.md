---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a7f6f3440e7fb3cd30380bc5af1f5572060e10a7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126019"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelTab -TeamId $teamId -ChannelId $channelId -ExpandProperty "teamsApp" -Filter "teamsApp/id eq 'com.microsoft.teamspace.tab.planner'" 

```