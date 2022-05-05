---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9ace3126a788d79deef8f950a1896125834432da
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206757"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    Action = "adminRemove"
    RoleDefinitionId = "8424c6f0-a189-499e-bbd0-26c1753c96d4"
    DirectoryScopeId = "/"
    PrincipalId = "071cc716-8147-4397-a5ba-b2105951cc0b"
}

New-MgRoleManagementDirectoryRoleEligibilityScheduleRequest -BodyParameter $params

```