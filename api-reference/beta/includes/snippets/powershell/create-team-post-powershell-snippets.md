---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 18cb757533ae8d0c326fddf56675d409c6f9e0e9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102395"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    "Template@odata.bind" = "https://graph.microsoft.com/beta/teamsTemplates('standard')"
    DisplayName = "My Sample Team"
    Description = "My Sample Team’s Description"
}

New-MgTeam -BodyParameter $params

```