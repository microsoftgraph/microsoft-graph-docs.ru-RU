---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 68b659682d7ea0476bca415bcea164f7fedf723f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120798"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    Description = "This is an updated description."
}

Update-MgComplianceEdiscoveryCaseTag -CaseId $caseId -TagId $tagId -BodyParameter $params

```