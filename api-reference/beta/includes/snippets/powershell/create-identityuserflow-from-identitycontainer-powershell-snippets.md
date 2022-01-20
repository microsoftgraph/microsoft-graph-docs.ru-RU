---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 84532a42076609dca9e1c7db148cf523ea0d573e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099646"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    Id = "Pol1"
    UserFlowType = "signUpOrSignIn"
    UserFlowTypeVersion = 1
}

New-MgIdentityUserFlow -BodyParameter $params

```