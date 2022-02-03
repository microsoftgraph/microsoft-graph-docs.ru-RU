---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 47bada10947232531edcfa5fac4868c7ced8657b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339730"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    "@odata.type" = "microsoft.graph.openTypeExtension"
    ExtensionName = "Com.Contoso.Referral"
    CompanyName = "Wingtip Toys"
    DealValue = 
    ExpirationDate = "2015-12-03T10:00:00.000Z"
}

# A UPN can also be used as -UserId.
New-MgUserMessageExtension -UserId $userId -MessageId $messageId -BodyParameter $params

```