---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 55c9e108d6011848717671d28838055cf3a4fd58
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121251"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Conditions = @{
        SignInRiskLevels = @(
            "high"
            "medium"
            "low"
        )
    }
}

Update-MgIdentityConditionalAccessPolicy -ConditionalAccessPolicyId $conditionalAccessPolicyId -BodyParameter $params

```