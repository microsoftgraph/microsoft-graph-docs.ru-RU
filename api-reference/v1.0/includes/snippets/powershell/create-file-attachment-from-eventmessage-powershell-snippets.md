---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aa2455c8c41cd9fccbb70935b7afee71ff786e55
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111029"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    "@odata.type" = "microsoft.graph.fileAttachment"
    Name = "name-value"
    ContentType = "contentType-value"
    IsInline = $false
    ContentLocation = "contentLocation-value"
    ContentBytes = "base64-contentBytes-value"
}

New-MgUserMessageAttachment -UserId $userId -MessageId $messageId -BodyParameter $params

```