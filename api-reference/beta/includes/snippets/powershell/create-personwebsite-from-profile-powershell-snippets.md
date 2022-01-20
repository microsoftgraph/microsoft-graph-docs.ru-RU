---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d2c45d2425b72f70c35996757445d1f2cf90cf7b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62123073"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Categories = @(
        "football"
    )
    DisplayName = "Lyn Damer"
    WebUrl = "www.lyndamer.no"
}

New-MgUserProfileWebsite -UserId $userId -BodyParameter $params

```