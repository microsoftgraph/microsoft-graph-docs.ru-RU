---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 55857d3890eaef1c92bfb785dd78a304852feb8e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127482"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Publisher = "International Association of Branding Management Publishing"
    ThumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg"
}

Update-MgUserProfilePublication -UserId $userId -ItemPublicationId $itemPublicationId -BodyParameter $params

```