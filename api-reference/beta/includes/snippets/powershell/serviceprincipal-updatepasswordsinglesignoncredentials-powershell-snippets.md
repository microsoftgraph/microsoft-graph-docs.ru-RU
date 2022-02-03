---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4913a04672b82788f62038ef3192fbdf3104782a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343970"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Id = "5793aa3b-cca9-4794-679a240f8b58"
    Credentials = @(
        @{
            FieldId = "param_username"
            Value = "myusername"
            Type = "username"
        }
        @{
            FieldId = "param_password"
            Value = "pa$$w0rd"
            Type = "password"
        }
    )
}

Update-MgServicePrincipalPasswordSingleSignOnCredentials -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```