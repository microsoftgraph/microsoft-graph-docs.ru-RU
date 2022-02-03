---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b0784183b0ffb2e38e1487a3faf804c5f4254bc8
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349331"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMessage -UserId $userId -MessageId $messageId -Property "subject,body,bodyPreview,uniqueBody" 

```