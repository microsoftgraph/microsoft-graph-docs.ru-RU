---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a250b6827d4a61aaa5194aa7dff306504a302ef
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350801"
---
```powershell

Import-Module Microsoft.Graph.Files

# A UPN can also be used as -UserId.
Get-MgUserDrive -UserId $userId

```