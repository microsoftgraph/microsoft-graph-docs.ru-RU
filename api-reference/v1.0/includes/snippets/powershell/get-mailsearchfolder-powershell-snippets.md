---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 53225b6a4be0a1e8d0429d352c78b1e37cd130cb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130274"
---
```powershell

Import-Module Microsoft.Graph.Mail

Get-MgUserMailFolder -UserId $userId -MailFolderId $mailFolderId

```