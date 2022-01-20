---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f1365fcf232e569cc5920d5c45804fe400997c54
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129835"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "Connected organization name"
    Description = "Connected organization description"
    IdentitySources = @(
        @{
            "@odata.type" = "#microsoft.graph.domainIdentitySource"
            DomainName = "example.com"
            DisplayName = "example.com"
        }
    )
    State = "proposed"
}

New-MgEntitlementManagementConnectedOrganization -BodyParameter $params

```