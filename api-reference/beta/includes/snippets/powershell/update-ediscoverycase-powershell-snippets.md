---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 479087caeee2b79a1b518d0d03c56c8fffbebc2d
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441870"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    DisplayName = "My Case 1 - Renamed"
    Description = "Updated description"
}

Update-MgSecurityCaseEdiscoveryCase -EdiscoveryCaseId $ediscoveryCaseId -BodyParameter $params

```