---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: af09dec4e84bcf9038e9398512644082b1f87d39
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62093758"
---
```powershell

Import-Module Microsoft.Graph.Planner

$params = @{
    SharedWith = @{
        "6463a5ce-2119-4198-9f2a-628761df4a62" = $true
        "D95e6152-f683-4d78-9ff5-67ad180fea4a" = $false
    }
    CategoryDescriptions = @{
        Category1 = "Indoors"
        Category3 = $null
    }
}

Update-MgPlannerPlanDetail -PlannerPlanId $plannerPlanId -BodyParameter $params

```