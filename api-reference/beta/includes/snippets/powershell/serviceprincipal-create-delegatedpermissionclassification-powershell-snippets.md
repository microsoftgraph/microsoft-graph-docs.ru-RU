---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 61c1a7f3de597da55fd722a8220ab24510262ca5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62093144"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    PermissionId = "e1fe6dd8-ba31-4d61-89e7-88639da4683d"
    PermissionName = "User.Read"
    Classification = "low"
}

New-MgServicePrincipalDelegatedPermissionClassification -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```