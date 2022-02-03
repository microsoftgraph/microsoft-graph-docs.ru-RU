---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6cd6a530b0e7bb89e32c617dd004cdcc56b4e582
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349914"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Description = "Lifetime Achievement award from the International Association of Branding Managers"
    DisplayName = "Lifetime Achievement Award For Excellence in Branding"
    IssuedDate = "Date"
    IssuingAuthority = "International Association of Branding Management"
    ThumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg"
    WebUrl = "https://www.iabm.io"
}

# A UPN can also be used as -UserId.
New-MgUserProfileAward -UserId $userId -BodyParameter $params

```