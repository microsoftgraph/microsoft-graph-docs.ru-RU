---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e77f3db11d06214bfbe723ccb9d67151737fe3f5
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351850"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    "@odata.type" = "#microsoft.graph.fileAttachment"
    Name = "smile"
    ContentBytes = "R0lGODdhEAYEAA7"
}

# A UPN can also be used as -UserId.
New-MgUserMessageAttachment -UserId $userId -MessageId $messageId -BodyParameter $params

```