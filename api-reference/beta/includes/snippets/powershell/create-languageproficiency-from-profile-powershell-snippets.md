---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ad01a7a90d211a0fbc5aa49627f17cec77aecb31
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351933"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    DisplayName = "Norwegian Bokmål"
    Tag = "nb-NO"
    Spoken = "nativeOrBilingual"
    Written = "nativeOrBilingual"
    Reading = "nativeOrBilingual"
}

# A UPN can also be used as -UserId.
New-MgUserProfileLanguage -UserId $userId -BodyParameter $params

```