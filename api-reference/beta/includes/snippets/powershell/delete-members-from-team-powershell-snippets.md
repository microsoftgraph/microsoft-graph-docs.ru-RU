---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 27012b635706303c666b8dbbacc4bb497211e64c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089348"
---
```powershell

Import-Module Microsoft.Graph.Teams

Remove-MgTeamMember -TeamId $teamId -ConversationMemberId $conversationMemberId

```