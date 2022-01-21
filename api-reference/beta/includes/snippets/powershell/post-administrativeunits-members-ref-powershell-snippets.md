---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 06a635f3265e4cb52fd7ff4b5b4411bd309ac507
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097406"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    "@odata.id" = "https://graph.microsoft.com/beta/groups/{id}"
}

New-MgAdministrativeUnitMemberByRef -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```