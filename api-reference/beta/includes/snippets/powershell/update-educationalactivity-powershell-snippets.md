---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 90eb8e914b8716082af91a6cb898d5c0249ce901
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352152"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Institution = @{
        Location = @{
            Type = "business"
            PostOfficeBox = $null
            Street = "12000 E Prospect Rd"
            City = "Fort Collins"
            State = "Colorado"
            CountryOrRegion = "USA"
            PostalCode = "80525"
        }
    }
}

# A UPN can also be used as -UserId.
Update-MgUserProfileEducationalActivity -UserId $userId -EducationalActivityId $educationalActivityId -BodyParameter $params

```