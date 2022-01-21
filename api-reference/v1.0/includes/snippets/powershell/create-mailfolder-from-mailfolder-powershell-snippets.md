---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 183c911131dfeabe2858c9403e46533e5b7a1a49
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117297"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    DisplayName = "displayName-value"
    IsHidden = $true
}

New-MgUserMailFolderChildFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```