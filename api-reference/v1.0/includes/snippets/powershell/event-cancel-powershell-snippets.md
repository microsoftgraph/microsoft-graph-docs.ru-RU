---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 24acff4e31f9cee66cc424faf7e5603937d0a42c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345547"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Comment = "Cancelling for this week due to all hands"
}

# A UPN can also be used as -UserId.
Stop-MgUserEvent -UserId $userId -EventId $eventId -BodyParameter $params

```