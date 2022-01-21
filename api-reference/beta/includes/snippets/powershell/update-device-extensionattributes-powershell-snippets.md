---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e684e3baa4d297895d24ce8d43989762978f7726
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096873"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    ExtensionAttributes = @{
        ExtensionAttribute1 = "BYOD-Device"
    }
}

Update-MgDevice -DeviceId $deviceId -BodyParameter $params

```