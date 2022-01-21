---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a4c7358f7f76ef2fcfc5e4eba310f6c793ec1f96
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115114"
---
```powershell

Import-Module Microsoft.Graph.Calendar

Remove-MgUserCalendarPermission -UserId $userId -CalendarPermissionId $calendarPermissionId

```