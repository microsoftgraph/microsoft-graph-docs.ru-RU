---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 611e5fb7498b04c0b8d99a3b2b14ecc07f9ed47c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351045"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Name = "name-value"
}

# A UPN can also be used as -UserId.
Update-MgUserCalendarGroup -UserId $userId -CalendarGroupId $calendarGroupId -BodyParameter $params

```