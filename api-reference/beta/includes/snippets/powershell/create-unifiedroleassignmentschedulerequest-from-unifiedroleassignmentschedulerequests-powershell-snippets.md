---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9a40d8940d67feecd571758b739730b6b72e96b9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098419"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    Action = "AdminAssign"
    Justification = "Assign User Admin to IT Helpdesk (User) group"
    RoleDefinitionId = "fdd7a751-b60b-444a-984c-02652fe8fa1c"
    DirectoryScopeId = "/"
    PrincipalId = "07706ff1-46c7-4847-ae33-3003830675a1"
    ScheduleInfo = @{
        StartDateTime = [System.DateTime]::Parse("2021-07-01T00:00:00Z")
        Expiration = @{
            Type = "NoExpiration"
        }
    }
}

New-MgRoleManagementDirectoryRoleAssignmentScheduleRequest -BodyParameter $params

```