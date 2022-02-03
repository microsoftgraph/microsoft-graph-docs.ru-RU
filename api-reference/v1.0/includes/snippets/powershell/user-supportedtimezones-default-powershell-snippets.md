---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 92b1a7c9af767ba9403559520e6e8fd3392c4274
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62345758"
---
```powershell

Import-Module Microsoft.Graph.Users.Functions

# A UPN can also be used as -UserId.
Invoke-MgTimeUserOutlook -UserId $userId

```