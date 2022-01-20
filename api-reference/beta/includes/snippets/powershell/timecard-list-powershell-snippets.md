---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f572a0aaa78b0b0ecc43f2d9c511cf62adb5cb82
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62108034"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamScheduleTimeCard -TeamId $teamId -Top 2 -Filter "state eq 'clockedOut'" 

```