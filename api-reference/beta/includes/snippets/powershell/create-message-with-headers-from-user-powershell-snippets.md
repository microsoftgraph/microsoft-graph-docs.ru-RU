---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2aa84cd22fb224bd8aa0958ede2b8b6c650a149a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095738"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    Subject = "9/8/2018: concert"
    Body = @{
        ContentType = "HTML"
        Content = "The group represents Washington."
    }
    ToRecipients = @(
        @{
            EmailAddress = @{
                Address = "AlexW@contoso.OnMicrosoft.com"
            }
        }
    )
    InternetMessageHeaders = @(
        @{
            Name = "x-custom-header-group-name"
            Value = "Washington"
        }
        @{
            Name = "x-custom-header-group-id"
            Value = "WA001"
        }
    )
}

New-MgUserMessage -UserId $userId -BodyParameter $params

```