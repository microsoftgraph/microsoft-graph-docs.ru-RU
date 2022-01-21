---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 97512313b268405f8f14e06188d62d58a5d7aa0c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121447"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    AssignedTo = "String"
    ClosedDateTime = [System.DateTime]::Parse("String (timestamp)")
    Comments = @(
        "String"
    )
    Feedback = "@odata.type: microsoft.graph.alertFeedback"
    Status = "@odata.type: microsoft.graph.alertStatus"
    Tags = @(
        "String"
    )
    VendorInformation = @{
        Provider = "String"
        Vendor = "String"
    }
}

Update-MgSecurityAlert -AlertId $alertId -BodyParameter $params

```