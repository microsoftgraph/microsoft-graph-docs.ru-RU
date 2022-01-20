---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3c0ef9e3d0222b6fef52157c91f74f0c9da2f493
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132487"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    ReceivedDateTime = [System.DateTime]::Parse("datetime-value")
    SentDateTime = [System.DateTime]::Parse("datetime-value")
    HasAttachments = $true
    Subject = "subject-value"
    Body = @{
        ContentType = ""
        Content = "content-value"
    }
    BodyPreview = "bodyPreview-value"
}

New-MgUserMailFolderMessage -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```