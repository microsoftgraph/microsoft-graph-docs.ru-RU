---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 736348bb92c4b6d39aa77a9eda76b263dd404577
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121673"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    DisplayName = "Vacation Plan"
}

Update-MgUserTodoList -UserId $userId -TodoTaskListId $todoTaskListId -BodyParameter $params

```