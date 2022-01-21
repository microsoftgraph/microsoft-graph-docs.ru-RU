---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fd5c4dfee684b2049eb698bd51fc1ba81ef4394c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110975"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Topic = "New Conversation Thread Topic"
    Posts = @(
        @{
            Body = @{
                ContentType = "html"
                Content = "this is body content"
            }
            NewParticipants = @(
                @{
                    EmailAddress = @{
                        Name = "Alex Darrow"
                        Address = "alexd@contoso.com"
                    }
                }
            )
        }
    )
}

New-MgGroupThread -GroupId $groupId -BodyParameter $params

```