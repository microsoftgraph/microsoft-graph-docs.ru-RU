---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e5560cf00ff42b60f3d1d8ee5a7730060a36a41b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118061"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    PasswordProfile = @{
        ForceChangePasswordNextSignIn = $false
        Password = "xWwvJ]6NMw+bWH-d"
    }
}

Update-MgUser -UserId $userId -BodyParameter $params

```