---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 300da59440515aeded59b3682834aa26f8ae3007
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348615"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    PasswordCredential = @{
        DisplayName = "Password friendly name"
    }
}

Add-MgServicePrincipalPassword -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```