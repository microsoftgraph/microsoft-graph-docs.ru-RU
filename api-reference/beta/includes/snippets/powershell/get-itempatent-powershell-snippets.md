---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 03c01b78e13a755d4813f1c2c5f6e87ff9f7279d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349554"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfilePatent -UserId $userId -ItemPatentId $itemPatentId

```