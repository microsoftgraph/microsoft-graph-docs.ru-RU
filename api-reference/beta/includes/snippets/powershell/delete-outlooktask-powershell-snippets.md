---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f1388858e0f298c9fec6122f8d1708d8b093d08e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352363"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Remove-MgUserOutlookTask -UserId $userId -OutlookTaskId $outlookTaskId

```