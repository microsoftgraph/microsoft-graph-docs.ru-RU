---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b659e9422de6f0d1d83ea4bf6f3dd0eda211ac3d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122128"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    DisplayName = "PassthroughAuthentication rollout policy"
    Description = "PassthroughAuthentication rollout policy"
    Feature = "passthroughAuthentication"
    IsEnabled = $true
    IsAppliedToOrganization = $false
}

New-MgPolicyFeatureRolloutPolicy -BodyParameter $params

```