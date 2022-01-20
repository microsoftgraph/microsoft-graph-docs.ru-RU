---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4f5a96bd10cdb5dc194530c29357ff6c92691dd2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101600"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "Architecture Discussion"
    Description = "This channel is where we debate all future architecture plans"
    MembershipType = "standard"
}

New-MgTeamChannel -TeamId $teamId -BodyParameter $params

```