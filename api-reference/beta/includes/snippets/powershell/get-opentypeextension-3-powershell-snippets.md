---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 111c1b5a3e25ee7ed8459f9743a95ca1b1aaf2e2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352222"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMessage -UserId $userId -MessageId $messageId -ExpandProperty "extensions(`$filter=id eq 'Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Referral')" 

```