---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 615ece547b432ae30f1cb0f67e964ececd494ba4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088094"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    AssignedTo = ""
    Comment = "control is reviewed"
    State = "Reviewed"
    VendorInformation = @{
        Provider = "SecureScore"
        ProviderVersion = $null
        SubProvider = $null
        Vendor = "Microsoft"
    }
}

Update-MgSecuritySecureScoreControlProfile -SecureScoreControlProfileId $secureScoreControlProfileId -BodyParameter $params

```