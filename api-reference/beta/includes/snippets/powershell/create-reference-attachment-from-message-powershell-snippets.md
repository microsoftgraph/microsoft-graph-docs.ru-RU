---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 545b577c5322bbeea00a7a5955f8287ff805e65b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62099470"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    "@odata.type" = "#microsoft.graph.referenceAttachment"
    Name = "Personal pictures"
    SourceUrl = "https://contoso.com/personal/mario_contoso_net/Documents/Pics"
    ProviderType = "oneDriveConsumer"
    Permission = "Edit"
    IsFolder = "True"
}

New-MgUserMessageAttachment -UserId $userId -MessageId $messageId -BodyParameter $params

```