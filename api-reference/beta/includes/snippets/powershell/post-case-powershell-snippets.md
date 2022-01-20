---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a532899f2b7d1d917d5eb114b23304dd91a75008
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100241"
---
```powershell

Import-Module Microsoft.Graph.Compliance

$params = @{
    DisplayName = "My Case 1"
}

New-MgComplianceEdiscoveryCase -BodyParameter $params

```