---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b41607451390d7d3470f2078b916802cbf3b8fac
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126180"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    DisplayName = "New display name"
}

Update-MgApplication -ApplicationId $applicationId -BodyParameter $params

```