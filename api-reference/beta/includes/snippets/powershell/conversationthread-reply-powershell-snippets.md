---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1cae168c2d95f7737443f26a62026132a67b30bc
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344565"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    Post = @{
        Body = @{
            ContentType = ""
            Content = "content-value"
        }
    }
}

Invoke-MgReplyGroupThread -GroupId $groupId -ConversationThreadId $conversationThreadId -BodyParameter $params

```