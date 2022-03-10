---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7ffbe816e6771eac4934d56a5b5cc355ca4b6bb8
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2022
ms.locfileid: "63416406"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Name = "jobGroup"
    DataType = "String"
    TargetObjects = @(
        "User"
    )
}

New-MgApplicationExtensionProperty -ApplicationId $applicationId -BodyParameter $params

```