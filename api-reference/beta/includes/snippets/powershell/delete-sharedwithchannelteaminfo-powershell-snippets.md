---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dcbc94a3948f8b7cddfd311ea7f11802e962b141
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65628988"
---
```powershell

Import-Module Microsoft.Graph.Teams

Remove-MgTeamChannelShared -TeamId $teamId -ChannelId $channelId -SharedWithChannelTeamInfoId $sharedWithChannelTeamInfoId

```