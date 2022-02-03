---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c7b4063eb33756c34a5facdc481b2ac83c255ccb
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341035"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

# A UPN can also be used as -UserId.
Revoke-MgUserSign -UserId $userId

```