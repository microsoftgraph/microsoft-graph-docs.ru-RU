---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7137652e76b4222ece301193ce3f1f577d4eb80c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101726"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    SelfServiceSignUp = @{
        IsEnabled = $true
    }
}

Update-MgPolicyAuthenticationFlowPolicy -BodyParameter $params

```