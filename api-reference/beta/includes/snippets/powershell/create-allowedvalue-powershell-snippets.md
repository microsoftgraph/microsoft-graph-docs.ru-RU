---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0c56d4c5b5f7513a5c8c9d643760715ea225cedd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62090736"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    Id = "Alpine"
    IsActive = "true"
}

New-MgDirectoryCustomSecurityAttributeDefinitionAllowedValue -CustomSecurityAttributeDefinitionId $customSecurityAttributeDefinitionId -BodyParameter $params

```