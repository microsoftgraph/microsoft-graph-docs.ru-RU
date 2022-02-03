---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 99f06da3685d3fb4a560ade7c6f4951ac0959520
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352035"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Name = "Leisure tasks"
}

# A UPN can also be used as -UserId.
New-MgUserOutlookTaskGroup -UserId $userId -BodyParameter $params

```