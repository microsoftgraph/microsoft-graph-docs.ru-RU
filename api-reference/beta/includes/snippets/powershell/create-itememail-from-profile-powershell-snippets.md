---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 79c7e41e07f8367754ddbc42d933d51f0196a2a3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132858"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Address = "Innocenty.Popov@adventureworks.com"
}

New-MgUserProfileEmail -UserId $userId -BodyParameter $params

```