---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4c6cfe782c53a8fb3aa8d4f69d4e0026c067eef3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106689"
---
```powershell

Import-Module Microsoft.Graph.DeviceManagement.Administration

Get-MgDeviceManagementVirtualEndpointUserSetting -CloudPcUserSettingId $cloudPcUserSettingId -ExpandProperty "assignments" 

```