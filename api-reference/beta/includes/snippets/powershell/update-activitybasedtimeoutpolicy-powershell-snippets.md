---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a4cc9eaf4316a6fbc8b744390ca69989751faf8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116927"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Definition = @(
        "definition-value"
    )
    DisplayName = "displayName-value"
    IsOrganizationDefault = $true
}

Update-MgPolicyActivityBasedTimeoutPolicy -ActivityBasedTimeoutPolicyId $activityBasedTimeoutPolicyId -BodyParameter $params

```