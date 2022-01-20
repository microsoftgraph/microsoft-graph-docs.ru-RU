---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c8b98803fd9201e1274ad0da64a9be523780fa90
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114694"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    "@odata.id" = "https://graph.microsoft.com/v1.0/users/{id}"
}

Set-MgUserManagerByRef -UserId $userId -BodyParameter $params

```