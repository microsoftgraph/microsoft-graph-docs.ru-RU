---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a10191441d0d24e18d77b09c594267db9893d409
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103407"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    Site = @{
        WebUrl = "https://contoso.sharepoint.com/sites/HumanResources"
    }
}

New-MgComplianceEdiscoveryCaseCustodianSiteSource -CaseId $caseId -CustodianId $custodianId -BodyParameter $params

```