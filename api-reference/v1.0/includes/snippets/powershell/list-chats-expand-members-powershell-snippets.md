---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cf239d00bcd1600d18c715bdf1ef6bdea8f05505
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134944"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgUserChat -UserId $userId -ExpandProperty "members" 

```