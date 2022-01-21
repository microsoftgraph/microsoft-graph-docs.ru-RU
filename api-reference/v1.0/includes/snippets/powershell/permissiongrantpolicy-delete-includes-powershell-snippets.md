---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c1861c308d380a72dcb894a3c90e3e300c230152
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134560"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Remove-MgPolicyPermissionGrantPolicyInclude -PermissionGrantPolicyId $permissionGrantPolicyId -PermissionGrantConditionSetId $permissionGrantConditionSetId

```