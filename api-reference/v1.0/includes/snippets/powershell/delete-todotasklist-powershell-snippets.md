---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 54b3e3a8302cd8f376a008f76094e5eef9f64666
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104317"
---
```powershell

Import-Module Microsoft.Graph.Users

Remove-MgUserTodoList -UserId $userId -TodoTaskListId $todoTaskListId

```