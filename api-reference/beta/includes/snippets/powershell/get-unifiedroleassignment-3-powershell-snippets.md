---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0d8ea7ca0014d99778b3ac91722ab8c31e2df4bd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135040"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

Get-MgRoleManagementCloudPcRoleAssignment -UnifiedRoleAssignmentMultipleId $unifiedRoleAssignmentMultipleId -ExpandProperty "roleDefinition" 

```