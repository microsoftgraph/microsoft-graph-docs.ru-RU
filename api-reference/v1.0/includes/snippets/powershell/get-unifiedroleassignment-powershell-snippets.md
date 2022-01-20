---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6b38124c0db594b1319d5998b8afffe062682944
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62087538"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

Get-MgRoleManagementDirectoryRoleAssignment -UnifiedRoleAssignmentId $unifiedRoleAssignmentId -ExpandProperty "roleDefinition,principal,directoryScope" 

```