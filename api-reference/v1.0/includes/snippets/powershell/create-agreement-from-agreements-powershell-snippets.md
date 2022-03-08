---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 18ec6f78cb1cb26f568c8cbd31a41d05e0152fc5
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336265"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "MSGraph Sample"
    IsViewingBeforeAcceptanceRequired = $true
    Files = @(
        @{
            FileName = "TOU.pdf"
            Language = "en"
            IsDefault = $true
            FileData = @{
                Data = [System.Text.Encoding]::ASCII.GetBytes("SGVsbG8gd29ybGQ=")
            }
        }
    )
}

New-MgIdentityGovernanceTermOfUseAgreement -BodyParameter $params

```