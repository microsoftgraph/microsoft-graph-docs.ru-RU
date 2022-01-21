---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 91f9f2ca62ae06d197511a968749d5be56d26f9b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127569"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    ClientSecret = "1111111111111"
}

Update-MgIdentityProvider -IdentityProviderId $identityProviderId -BodyParameter $params

```