---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8f32c59375a22628d4299e66fdfef3d0ebfa1139
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351424"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfileWebsite -UserId $userId -PersonWebsiteId $personWebsiteId

```