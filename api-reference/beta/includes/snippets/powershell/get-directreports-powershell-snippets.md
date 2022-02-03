---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7805c916d8dacf2b9ddb239d58c5b74d2fa17605
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350324"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserDirectReport -UserId $userId

```