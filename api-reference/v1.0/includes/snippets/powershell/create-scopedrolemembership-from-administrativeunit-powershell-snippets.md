---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e4ff0408deb25f6dca9cfdfaf0200648691a79fc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088887"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    RoleId = "roleId-value"
    RoleMemberInfo = @{
        Id = "id-value"
    }
}

New-MgDirectoryAdministrativeUnitScopedRoleMember -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```