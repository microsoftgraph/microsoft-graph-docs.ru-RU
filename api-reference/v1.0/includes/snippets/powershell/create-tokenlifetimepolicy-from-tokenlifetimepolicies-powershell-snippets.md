---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ddf51281ffe4c7028645fa1da346ea6e0f120ae4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128232"
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

New-MgPolicyTokenLifetimePolicy -BodyParameter $params

```