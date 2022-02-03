---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6665b4457d341f6242e414e15c394f70d27b341b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344537"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUser -UserId $userId

```