---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9eefd0e484b1fbd0c64ae68336dfbc346071cc4f
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340048"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Message = @{
        ToRecipients = @(
            @{
                EmailAddress = @{
                    Address = "samanthab@contoso.onmicrosoft.com"
                    Name = "Samantha Booth"
                }
            }
            @{
                EmailAddress = @{
                    Address = "randiw@contoso.onmicrosoft.com"
                    Name = "Randi Welch"
                }
            }
        )
    }
    Comment = "Samantha, Randi, would you name the group please?"
}

# A UPN can also be used as -UserId.
Invoke-MgReplyUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```