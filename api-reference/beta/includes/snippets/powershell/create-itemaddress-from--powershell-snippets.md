---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c16ef3bc158436a3adb3ce72bad5bec4810a743a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349606"
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

# A UPN can also be used as -UserId.
New-MgUserProfileAddress -UserId $userId -BodyParameter $params

```