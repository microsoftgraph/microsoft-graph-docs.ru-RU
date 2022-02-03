---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8a443ef8a4a3874c2bc65dbeee0dfd4a85fd5b81
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349504"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Get-MgUserEvent -UserId $userId -Property "subject,body,bodyPreview" 

```