---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c371f355094cb8d810bfeb810e49105f9513d7bf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131111"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMailFolderChildFolder -UserId $userId -MailFolderId $mailFolderId -Includehiddenfolders true 

```