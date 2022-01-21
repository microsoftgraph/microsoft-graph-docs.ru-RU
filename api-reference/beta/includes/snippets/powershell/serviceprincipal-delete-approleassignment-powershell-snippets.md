---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a1e3b51e091c3421c81f46aed478ce324cbc44f1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115849"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgServicePrincipalAppRoleAssignment -ServicePrincipalId $servicePrincipalId -AppRoleAssignmentId $appRoleAssignmentId

```