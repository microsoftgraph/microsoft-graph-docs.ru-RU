---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2d42372d82bef4b5f1645fd4961fa1c2376daa0a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347495"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "Library Assist"
    Description = "Self help community for library"
    MailNickname = "libassist"
    PartsToClone = "apps,tabs,settings,channels,members"
    Visibility = "public"
}

Copy-MgTeam -TeamId $teamId -BodyParameter $params

```