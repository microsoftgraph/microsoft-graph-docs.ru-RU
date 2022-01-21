---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7f413e32cdb6eac15aef0e3dcc7f5ba187659895
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115572"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    Description = "description-updated"
}

Update-MgSecurityTiIndicator -TiIndicatorId $tiIndicatorId -BodyParameter $params

```