---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6fd43cbdb92e3c84cb54b63ddfc4cd3e6bd1357d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113658"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    ExternalUserLifecycleAction = "None"
}

Update-MgEntitlementManagementSetting -BodyParameter $params

```