---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 07c14ea383714922c538ade0867747f4dd96dd5b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131333"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    Email = "adelev@contoso.com"
    IncludedSources = "mailbox"
}

New-MgComplianceEdiscoveryCaseLegalHoldUserSource -CaseId $caseId -LegalHoldId $legalHoldId -BodyParameter $params

```