---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a9aac576283102be117b8294872149ea207b679c
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351995"
---
```powershell

Import-Module Microsoft.Graph.Sites

# A UPN can also be used as -UserId.
Get-MgUserFollowedSite -UserId $userId

```