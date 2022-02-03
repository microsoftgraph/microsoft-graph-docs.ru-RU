---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8a503fb6ba88eab58fc29aef4d67700fe2b6b221
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351931"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

# A UPN can also be used as -UserId.
Remove-MgUserOnlineMeetingRegistration -UserId $userId -OnlineMeetingId $onlineMeetingId

```