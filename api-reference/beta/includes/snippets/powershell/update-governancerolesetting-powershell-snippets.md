---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ffeb3fc7b31d050b110e19d333e9b9b8c88c6a42
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62108817"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    AdminEligibleSettings = @(
        @{
            RuleIdentifier = "ExpirationRule"
            Setting = "{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}"
        }
    )
}

Update-MgPrivilegedAccessRoleSetting -PrivilegedAccessId $privilegedAccessId -GovernanceRoleSettingId $governanceRoleSettingId -BodyParameter $params

```