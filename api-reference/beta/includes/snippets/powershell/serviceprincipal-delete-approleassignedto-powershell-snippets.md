---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5b31d12594c4ecb5e463849602c5d726dc4db00b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125452"
---
```powershell

Import-Module Microsoft.Graph.Applications

Remove-MgServicePrincipalAppRoleAssignedTo -ServicePrincipalId $servicePrincipalId -AppRoleAssignmentId $appRoleAssignmentId

```