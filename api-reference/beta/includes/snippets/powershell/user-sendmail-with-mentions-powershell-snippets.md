---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 18bce75d3a9588071d9fec216d9c8f9e1da511a3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340081"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Message = @{
        Subject = "Project kickoff"
        ToRecipients = @(
            @{
                EmailAddress = @{
                    Name = "Samantha Booth"
                    Address = "samanthab@contoso.onmicrosoft.com"
                }
            }
        )
        Mentions = @(
            @{
                Mentioned = @{
                    Name = "Dana Swope"
                    Address = "danas@contoso.onmicrosoft.com"
                }
            }
        )
    }
}

# A UPN can also be used as -UserId.
Send-MgUserMail -UserId $userId -BodyParameter $params

```