---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 21087e271a17a5b881d18728fae2d218ed277511
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347207"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Actions

$params = @{
    "@odata.type" = "#microsoft.graph.cloudPcProvisioningPolicyAssignment"
    Assignments = @(
        @{
            Id = "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
            Target = @{
                "@odata.type" = "microsoft.graph.cloudPcManagementGroupAssignmentTarget"
                GroupId = "64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
            }
        }
    )
}

Set-MgDeviceManagementVirtualEndpointProvisioningPolicy -CloudPcProvisioningPolicyId $cloudPcProvisioningPolicyId -BodyParameter $params

```