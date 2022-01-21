---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ce70d3a76075aa4841cc8fa407570b3584957455
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131375"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    Email = "AdeleV@contoso.com"
    ApplyHoldToSources = "true"
}

New-MgComplianceEdiscoveryCaseCustodian -CaseId $caseId -BodyParameter $params

```