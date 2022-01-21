---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ee144b706e6c2e87a4059029a635a4b4d2359699
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096244"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    MarketingNotificationEmails = @(
        "marketing@contoso.com"
    )
    PrivacyProfile = @{
        ContactEmail = "alice@contoso.com"
        StatementUrl = "https://contoso.com/privacyStatement"
    }
    SecurityComplianceNotificationMails = @(
        "security@contoso.com"
    )
    SecurityComplianceNotificationPhones = @(
        "(123) 456-7890"
    )
    TechnicalNotificationMails = @(
        "tech@contoso.com"
    )
}

Update-MgOrganization -OrganizationId $organizationId -BodyParameter $params

```