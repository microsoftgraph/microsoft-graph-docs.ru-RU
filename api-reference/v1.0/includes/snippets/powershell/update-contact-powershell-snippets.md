---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 09952b30a1fbeff90b29679d8b5500cf880c755a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352239"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

$params = @{
    HomeAddress = @{
        Street = "123 Some street"
        City = "Seattle"
        State = "WA"
        PostalCode = "98121"
    }
    Birthday = [System.DateTime]::Parse("1974-07-22")
}

# A UPN can also be used as -UserId.
Update-MgUserContact -UserId $userId -ContactId $contactId -BodyParameter $params

```