---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1a6dfd88879e33ed4de90907fe60ee62ba270644
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62093682"
---
```powershell

Import-Module Microsoft.Graph.Planner

$params = @{
    OrderHint = "A6673H Ejkl!"
}

Update-MgPlannerTaskProgressTaskBoardFormat -PlannerTaskId $plannerTaskId -BodyParameter $params

```