---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 00ad654c53ed76d086d2eb79ad66b56ecfa95447
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136897"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Definition = @(
        "definition-value"
    )
    DisplayName = "displayName-value"
    IsOrganizationDefault = $true
}

Update-MgPolicyTokenLifetimePolicy -TokenLifetimePolicyId $tokenLifetimePolicyId -BodyParameter $params

```