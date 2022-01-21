---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5a0bb851c5fa55e3293c6c766cb38e413e37e241
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102856"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

Get-MgUserOnlineMeetingRegistration -UserId $userId -OnlineMeetingId $onlineMeetingId -ExpandProperty "microsoft.graph.meetingRegistration/customQuestions" 

```