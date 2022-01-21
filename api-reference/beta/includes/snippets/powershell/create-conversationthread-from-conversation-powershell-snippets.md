---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1fc2f4d396f91ab33e43d930c5d1dcee9b92884f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106486"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Topic = "Take your wellness days and rest"
    Posts = @(
        @{
            Body = @{
                ContentType = "html"
                Content = "Waiting for the summer holidays."
            }
        }
    )
}

New-MgGroupConversationThread -GroupId $groupId -ConversationId $conversationId -BodyParameter $params

```