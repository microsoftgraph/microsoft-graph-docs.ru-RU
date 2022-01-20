---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 68cebb9d552e6ec51ee3209f1a1c73c3891aa126
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089621"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Name = "Leisure tasks"
}

New-MgUserOutlookTaskGroup -UserId $userId -BodyParameter $params

```