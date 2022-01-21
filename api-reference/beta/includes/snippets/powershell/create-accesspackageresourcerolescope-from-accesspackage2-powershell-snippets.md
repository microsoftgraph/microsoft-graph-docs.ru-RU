---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 47685b475f2f5e5a68ffa6a0bf42a91ffbd06cef
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097515"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    AccessPackageResourceRole = @{
        OriginId = "4"
        OriginSystem = "SharePointOnline"
        AccessPackageResource = @{
            Id = "53c71803-a0a8-4777-aecc-075de8ee3991"
        }
    }
    AccessPackageResourceScope = @{
        Id = "5ae0ae7c-d0a5-42aa-ab37-1f15e9a61d33"
        OriginId = "https://microsoft.sharepoint.com/portals/Community"
        OriginSystem = "SharePointOnline"
    }
}

New-MgEntitlementManagementAccessPackageResourceRoleScope -AccessPackageId $accessPackageId -BodyParameter $params

```