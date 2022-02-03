---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3d1fe3e959728389e0526ced8f637f677623597a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341736"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    DestinationTaskListId = "AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFsPFj7gQqFxG"
}

# A UPN can also be used as -UserId.
Move-MgUserTaskListTask -UserId $userId -BaseTaskListId $baseTaskListId -BaseTaskId $baseTaskId -BodyParameter $params

```