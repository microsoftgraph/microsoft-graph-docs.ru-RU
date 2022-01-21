---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b892f549dd3792bd0b6fb3e78b5467b6ba6f0504
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62120054"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
    Description = "An example custom role"
    DisplayName = "ExampleCustomRole"
    RolePermissions = @(
        @{
            AllowedResourceActions = @(
                "Microsoft.CloudPC/CloudPCs/Read"
            )
        }
    )
    Condition = "null"
}

New-MgRoleManagementCloudPcRoleDefinition -BodyParameter $params

```