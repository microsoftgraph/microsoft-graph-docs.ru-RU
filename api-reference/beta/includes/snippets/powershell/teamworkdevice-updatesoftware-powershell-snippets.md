---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ce9d161432631f5c7dac7f38e125311c814bab1d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348412"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    SoftwareType = "teamsClient"
    SoftwareVersion = "1.0.96.22"
}

Update-MgTeamworkDeviceSoftware -TeamworkDeviceId $teamworkDeviceId -BodyParameter $params

```