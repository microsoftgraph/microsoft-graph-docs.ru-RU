---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4a1b60d3211d0eb3ba203c718addf3514de6addd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088438"
---
```powershell

Import-Module Microsoft.Graph.Planner

$params = @{
    Name = "Development"
}

Update-MgPlannerBucket -PlannerBucketId $plannerBucketId -BodyParameter $params

```