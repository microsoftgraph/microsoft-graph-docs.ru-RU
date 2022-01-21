---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e9a8cc29248ad410d03e7346b28d7e9ab404fe63
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114392"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Name = "extensionName"
    DataType = "string"
    TargetObjects = @(
        "Application"
    )
}

New-MgApplicationExtensionProperty -ApplicationId $applicationId -BodyParameter $params

```