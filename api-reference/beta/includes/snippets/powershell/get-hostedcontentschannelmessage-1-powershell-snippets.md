---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ba5a0af26977ebe010e2e84f6893e3ed9adced56
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123987"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelMessageHostedContent -TeamId $teamId -ChannelId $channelId -ChatMessageId $chatMessageId

```