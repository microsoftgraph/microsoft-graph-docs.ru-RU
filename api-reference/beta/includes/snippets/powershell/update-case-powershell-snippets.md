---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3942beae760017a28c2399749f7272c31a728660
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133874"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    DisplayName = "My Case 1 - Renamed"
    Description = "Updated description"
    ExternalId = "Updated externalId"
}

Update-MgComplianceEdiscoveryCase -CaseId $caseId -BodyParameter $params

```