---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bdd811285af96a988214b164cb6af2bb113efbe2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112474"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    IssuingAuthority = "International Association of Branding Management"
    ThumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg"
}

Update-MgUserProfileAward -UserId $userId -PersonAwardId $personAwardId -BodyParameter $params

```