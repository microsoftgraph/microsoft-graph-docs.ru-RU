---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ae7fe460d062b0f5895dd3006c0f4766319e2cca
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134425"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    "@odata.type" = "#microsoft.graph.unifiedRoleAssignment"
    PrincipalId = "6b937a9d-c731-465b-a844-2d5b5368c161"
    RoleDefinitionId = "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3"
    DirectoryScopeId = "/661e1310-bd76-4795-89a7-8f3c8f855bfc"
}

New-MgRoleManagementDirectoryRoleAssignment -BodyParameter $params

```