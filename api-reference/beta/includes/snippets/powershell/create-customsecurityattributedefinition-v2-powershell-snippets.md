---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: af5bf08b95bac5db948b27b25dfd666b2053c6d9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106346"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    AttributeSet = "Engineering"
    Description = "Active projects for user"
    IsCollection = $true
    IsSearchable = $true
    Name = "Project"
    Status = "Available"
    Type = "String"
    UsePreDefinedValuesOnly = $true
}

New-MgDirectoryCustomSecurityAttributeDefinition -BodyParameter $params

```