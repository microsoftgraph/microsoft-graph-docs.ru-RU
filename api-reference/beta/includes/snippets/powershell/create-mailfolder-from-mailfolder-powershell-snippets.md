---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c5561626b19a78ed4c37c4094c6f3d5fc7e88544
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349817"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    DisplayName = "displayName-value"
    IsHidden = $true
}

# A UPN can also be used as -UserId.
New-MgUserMailFolderChildFolder -UserId $userId -MailFolderId $mailFolderId -BodyParameter $params

```