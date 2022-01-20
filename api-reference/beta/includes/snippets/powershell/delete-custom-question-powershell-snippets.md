---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 323698be19aa211712a2810dca06b23c7fd8ca6c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102811"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

Remove-MgUserOnlineMeetingRegistrationCustomQuestion -UserId $userId -OnlineMeetingId $onlineMeetingId -MeetingRegistrationQuestionId $meetingRegistrationQuestionId

```