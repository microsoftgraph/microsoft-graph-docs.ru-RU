---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ee45a832abc29ffa49995d3c381d12e7346fdd59
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131500"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

Get-MgDeviceManagementVirtualEndpointProvisioningPolicy -CloudPcProvisioningPolicyId $cloudPcProvisioningPolicyId -ExpandProperty "assignments" 

```