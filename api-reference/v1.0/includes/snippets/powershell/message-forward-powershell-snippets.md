---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e3792df0b999583bba90ea15e8d95662e9aafebe
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342359"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Comment = "comment-value"
    ToRecipients = @(
        @{
            EmailAddress = @{
                Name = "name-value"
                Address = "address-value"
            }
        }
    )
}

# A UPN can also be used as -UserId.
Invoke-MgForwardUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```