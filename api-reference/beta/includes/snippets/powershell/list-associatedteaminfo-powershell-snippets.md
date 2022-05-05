---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c283ced9cad7a5f76361fbe4fc1ee669ab04f8c5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203719"
---
```powershell

Import-Module Microsoft.Graph.Teams

# A UPN can also be used as -UserId.
Get-MgUserTeamworkAssociatedTeam -UserId $userId

```