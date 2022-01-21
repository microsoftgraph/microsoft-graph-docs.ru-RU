---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f64cf63469b1f242ba81dd561e8ab03183df74d8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104750"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMailFolderMessage -UserId $userId -MailFolderId $mailFolderId

```