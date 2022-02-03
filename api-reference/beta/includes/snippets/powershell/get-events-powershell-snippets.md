---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 14d0e92e5b8dbd4fe0a3bfb1fc968e49f5fededc
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349822"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Get-MgUserEvent -UserId $userId -Property "subject,body,bodyPreview,organizer,attendees,start,end,location" 

```