---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5ffc463c1febd705d40204f09a893a7252b28733
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115464"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    WebUrl = "https://microsoft.com"
    ApplicationName = "Microsoft"
    DisplayName = "Microsoft"
    ExternalId = "dk9cddce2-dce2-f9dd-e2dc-cdf9e2dccdf9"
}

New-MgUserTodoListTaskLinkedResource -UserId $userId -TodoTaskListId $todoTaskListId -TodoTaskId $todoTaskId -BodyParameter $params

```