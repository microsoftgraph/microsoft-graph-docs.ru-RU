---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 662f6a3cce7d097440eff62b855d54c3e8704dbb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101639"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannel -TeamId $teamId -Filter "membershipType eq 'private'" 

```