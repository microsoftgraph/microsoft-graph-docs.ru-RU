---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 798fbf2d907e61906684c0d677b6a8606d72e3f6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351513"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

# A UPN can also be used as -UserId.
Get-MgUserAuthenticationSoftwareOathMethod -UserId $userId

```