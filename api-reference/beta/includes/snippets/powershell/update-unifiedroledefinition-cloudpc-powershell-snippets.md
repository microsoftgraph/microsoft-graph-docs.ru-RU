---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 401dd47a40ff016d6fdbf5d3ae9f70aaab2466b3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62089160"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    Description = "Update basic properties and permission of application registrations"
    DisplayName = "ExampleCustomRole"
    RolePermissions = @(
        @{
            AllowedResourceActions = @(
                "Microsoft.CloudPC/CloudPCs/Read"
                "Microsoft.CloudPC/CloudPCs/Reprovision"
            )
        }
    )
}

Update-MgRoleManagementCloudPcRoleDefinition -UnifiedRoleDefinitionId $unifiedRoleDefinitionId -BodyParameter $params

```