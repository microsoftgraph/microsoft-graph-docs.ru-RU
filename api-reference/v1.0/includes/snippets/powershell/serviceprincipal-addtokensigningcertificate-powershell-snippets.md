---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: eb73d5a8d98a4dd367ca772e8df392addf5cb50a
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333241"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    DisplayName = "CN=customDisplayName"
    EndDateTime = [System.DateTime]::Parse("2024-01-25T00:00:00Z")
}

Add-MgServicePrincipalTokenSigningCertificate -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```