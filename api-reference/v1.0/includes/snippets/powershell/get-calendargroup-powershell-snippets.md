---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bafedf8271bce537a84b4793e7b43d5f8aa29e6d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350998"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Get-MgUserCalendarGroup -UserId $userId -CalendarGroupId $calendarGroupId

```