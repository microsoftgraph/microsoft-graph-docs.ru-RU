---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 67f1d895a75fc8491bb837566437c390687ce878
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350284"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

# A UPN can also be used as -UserId.
Get-MgUserOnlineMeetingAttendeeReport -UserId $userId -OnlineMeetingId $onlineMeetingId

```