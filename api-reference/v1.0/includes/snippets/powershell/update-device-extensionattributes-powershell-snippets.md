---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f397c4254185b91918e26f65ccf9165256902d29
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098000"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
}

Update-MgDevice -DeviceId $deviceId -BodyParameter $params

```