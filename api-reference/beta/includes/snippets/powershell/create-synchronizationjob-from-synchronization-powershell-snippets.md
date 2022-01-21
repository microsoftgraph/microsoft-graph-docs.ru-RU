---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7c0154b739688c6584e2128ed01084f2620c7b13
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105303"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    TemplateId = "BoxOutDelta"
}

New-MgServicePrincipalSynchronizationJob -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```