---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 389d921c2d404c882b3fdc71180e5ca7925136c3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348537"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    GroupId = "ffffffff-ffff-ffff-ffff-ffffffffffff"
}

Invoke-MgRenewGroupLifecyclePolicy -BodyParameter $params

```