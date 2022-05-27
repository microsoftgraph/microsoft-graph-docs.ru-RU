---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 10a66b7bcc90ff1eb1308706cef6dd27d718799e
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694987"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    AllowedCloudEndpoints = @(
        "microsoftonline.us"
        "partner.microsoftonline.cn"
    )
}

Update-MgPolicyCrossTenantAccessPolicy -BodyParameter $params

```