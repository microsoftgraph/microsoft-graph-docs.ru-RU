---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dfb757554ee191a34035622fdbd07605f7ed4735
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352750"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMailFolderChildFolder -UserId $userId -MailFolderId $mailFolderId -Includehiddenfolders true 

```