---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e3b8d89005ba653c9cab7f0c725ba3833decdd60
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344279"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    ToRecipients = @(
        @{
            EmailAddress = @{
                Address = "danas@contoso.onmicrosoft.com"
                Name = "Dana Swope"
            }
        }
    )
    Comment = "Dana, hope you can make this meeting."
}

# A UPN can also be used as -UserId.
Invoke-MgForwardUserEvent -UserId $userId -EventId $eventId -BodyParameter $params

```