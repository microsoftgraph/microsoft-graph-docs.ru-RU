---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8af84732dffcf0383f476f938caa814e703dbd57
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096371"
---
```powershell

Import-Module Microsoft.Graph.People

Remove-MgUserProfileEmail -UserId $userId -ItemEmailId $itemEmailId

```