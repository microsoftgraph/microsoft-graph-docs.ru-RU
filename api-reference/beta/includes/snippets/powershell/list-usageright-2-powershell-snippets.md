---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 43ed9036a56ed07a936676850f40e7a4b1bd29ce
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090713"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Get-MgDeviceUsageRights -DeviceId $deviceId -Filter "state in ('active', 'suspended') and serviceIdentifier in ('ABCD')" 

```