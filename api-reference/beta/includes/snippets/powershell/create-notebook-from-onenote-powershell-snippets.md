---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 22b3b19eb70b1e36cae6d34353af5fce14b1a0d4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135448"
---
```powershell

Import-Module Microsoft.Graph.Notes

$params = @{
    DisplayName = "My Private notebook"
}

New-MgUserOnenoteNotebook -UserId $userId -BodyParameter $params

```