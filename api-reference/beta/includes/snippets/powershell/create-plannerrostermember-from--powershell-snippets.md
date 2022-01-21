---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 580aa6134ccde0bdff4500f751c16bd4f8201c35
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62108419"
---
```powershell

Import-Module Microsoft.Graph.Planner

$params = @{
    "@odata.type" = "#microsoft.graph.plannerRosterMember"
    UserId = "String"
}

New-MgPlannerRosterMember -PlannerRosterId $plannerRosterId -BodyParameter $params

```