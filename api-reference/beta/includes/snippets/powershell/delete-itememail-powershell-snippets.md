---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f00a6f308a06dc07c557707b3a0a222c9e6ad486
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350588"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfileEmail -UserId $userId -ItemEmailId $itemEmailId

```