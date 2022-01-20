---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a48f86b57d2f1d4a48f25924e6117dfc40d6d45
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62112397"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Nickname = "Kesha"
}

Update-MgUserProfileName -UserId $userId -PersonNameId $personNameId -BodyParameter $params

```