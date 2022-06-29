---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c3c16b5c7527fde8cfd5164c4f25ad6555ab4830
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442410"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

Remove-MgDeviceRegisteredOwnerByRef -DeviceId $deviceId -DirectoryObjectId $directoryObjectId

```