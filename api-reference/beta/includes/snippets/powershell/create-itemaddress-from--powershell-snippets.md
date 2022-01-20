---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ae146b1d5d31024811f79de722df388261d2c87f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135309"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    DisplayName = "Home"
    Detail = @{
        Type = "home"
        PostOfficeBox = $null
        Street = "221B Baker Street"
        City = "London"
        State = $null
        CountryOrRegion = "United Kingdom"
        PostalCode = "E14 3TD"
    }
}

New-MgUserProfileAddress -UserId $userId -BodyParameter $params

```