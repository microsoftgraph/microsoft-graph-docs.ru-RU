---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 210e007dd3432d0d7e891945c053030f031feedd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091775"
---
```powershell

Import-Module Microsoft.Graph.SchemaExtensions

$params = @{
    Id = "graphlearn_courses"
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