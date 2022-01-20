---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d215fdf2b7411d22041d260481f792a10a266e1c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118670"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    AllowedAudiences = "organization"
}

Update-MgUserProfileNote -UserId $userId -PersonAnnotationId $personAnnotationId -BodyParameter $params

```