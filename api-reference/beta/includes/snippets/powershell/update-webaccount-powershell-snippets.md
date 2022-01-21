---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ff401bc157ebc0fdbce9e2cf85f2453a54141f63
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101978"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    WebUrl = "https://github.com/innocenty.popov"
}

Update-MgUserProfileWebAccount -UserId $userId -WebAccountId $webAccountId -BodyParameter $params

```