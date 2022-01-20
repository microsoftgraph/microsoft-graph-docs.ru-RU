---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 59b873a35572ed871c98594846a69859cd1aa970
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100697"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    IsGroupOwnerManagementEnabled = $true
}

Update-MgPolicyAccessReviewPolicy -BodyParameter $params

```