---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cc1e32df57c4ffad68144777ab768b90a75a0cd6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342764"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    WebUrl = "webUrl value"
}

# A UPN can also be used as -UserId.
Get-MgUserOnenoteNotebookFromWebUrl -UserId $userId -BodyParameter $params

```