---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c46e0d150e9dd75bfc48c15dc8b2413db6c463b8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129012"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelMessageReply -TeamId $teamId -ChannelId $channelId -ChatMessageId $chatMessageId -ChatMessageId1 $chatMessageId1

```