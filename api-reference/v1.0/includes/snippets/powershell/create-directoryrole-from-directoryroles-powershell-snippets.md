---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 840bdc0e1f86a058459abf4a4e4d2df07a6863fc
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117731"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    RoleTemplateId = "fe930be7-5e62-47db-91af-98c3a49a38b1"
}

New-MgDirectoryRole -BodyParameter $params

```