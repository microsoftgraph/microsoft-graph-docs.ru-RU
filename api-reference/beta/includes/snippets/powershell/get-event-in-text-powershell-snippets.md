---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c66076ffe79facf8c48967b0cc529f48bdfab4af
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351763"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Get-MgUserEvent -UserId $userId -EventId $eventId -Property "subject,body,bodyPreview" 

```