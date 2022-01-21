---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a835c7bd2b3ef5f1a9ca82c9b9cbe5638888fa8a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127447"
---
```powershell

Import-Module Microsoft.Graph.Mail

Remove-MgUserMailFolder -UserId $userId -MailFolderId $mailFolderId

```