---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c95ff962cb482791e09c0512bb2e4fb6b1822005
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136189"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    "@odata.type" = "#microsoft.graph.itemAttachment"
    Name = "Holiday event"
    Item = @{
        "@odata.type" = "microsoft.graph.event"
        Subject = "Discuss gifts for children"
    }
}

New-MgUserEventAttachment -UserId $userId -EventId $eventId -BodyParameter $params

```