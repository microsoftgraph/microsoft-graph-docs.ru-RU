---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 547008e08eeb3b45ca884be9e4f0680c7cf3db7b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129013"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelMessage -TeamId $teamId -ChannelId $channelId -ChatMessageId $chatMessageId

```