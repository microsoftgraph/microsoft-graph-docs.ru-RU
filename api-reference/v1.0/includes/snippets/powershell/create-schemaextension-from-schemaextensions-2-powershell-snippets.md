---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c50f1e8aeab0273dc35d008bdda0b230c3b1cae4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091776"
---
```powershell

Import-Module Microsoft.Graph.SchemaExtensions

$params = @{
    Id = "courses"
    Description = "Graph Learn training courses extensions"
    TargetTypes = @(
        "Group"
    )
    Properties = @(
        @{
            Name = "courseId"
            Type = "Integer"
        }
        @{
            Name = "courseName"
            Type = "String"
        }
        @{
            Name = "courseType"
            Type = "String"
        }
    )
}

New-MgSchemaExtension -BodyParameter $params

```