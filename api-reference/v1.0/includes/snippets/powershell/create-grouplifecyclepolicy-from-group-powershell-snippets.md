---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 902e86391cd1f8bef8c50fe9290e85688721ab2e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130373"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    GroupLifetimeInDays = 100
    ManagedGroupTypes = "Selected"
    AlternateNotificationEmails = "admin@contoso.com"
}

New-MgGroupLifecyclePolicy -BodyParameter $params

```