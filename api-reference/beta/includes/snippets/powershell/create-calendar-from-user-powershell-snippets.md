---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1ea122d6b211703df2ea40ce5fde5ba4a768b99c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102047"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    Name = "Volunteer"
}

New-MgUserCalendar -UserId $userId -BodyParameter $params

```