---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b07d6d564193188945cfc38bd8ed8b4685b06b3c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62093844"
---
```powershell

Import-Module Microsoft.Graph.Planner

$params = @{
    "@odata.type" = "#microsoft.graph.plannerRoster"
}

New-MgPlannerRoster -BodyParameter $params

```