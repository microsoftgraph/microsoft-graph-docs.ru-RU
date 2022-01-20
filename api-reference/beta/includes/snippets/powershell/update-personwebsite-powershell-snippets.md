---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3505f0378eac30fbc326ee701e405d3c8308089d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112383"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Description = "Lyn Damer play in the Women's 1st Division (Toppserien) in Norway"
}

Update-MgUserProfileWebsite -UserId $userId -PersonWebsiteId $personWebsiteId -BodyParameter $params

```