---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6b61399c8a59902f3053f4293b96bacefab3c468
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089523"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "testprogram3 new name"
}

Update-MgProgram -ProgramId $programId -BodyParameter $params

```