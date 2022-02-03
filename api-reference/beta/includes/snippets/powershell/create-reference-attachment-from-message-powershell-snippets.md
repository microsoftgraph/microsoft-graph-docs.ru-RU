---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7b256764dc45a09e0418d075123e0eaacf4c4b65
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350308"
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

# A UPN can also be used as -UserId.
New-MgUserMessageAttachment -UserId $userId -MessageId $messageId -BodyParameter $params

```