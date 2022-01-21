---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fb2267ace18430d376b1c9a1f4b4f17308b8f066
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129765"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Type = "other"
}

Update-MgUserProfilePhone -UserId $userId -ItemPhoneId $itemPhoneId -BodyParameter $params

```