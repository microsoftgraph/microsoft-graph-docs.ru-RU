---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 119943db37e1d7c80d7a9c6d94ea8d3b5fa48eec
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128967"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    Body = @{
        Content = "Hello world"
    }
}

New-MgChatMessage -ChatId $chatId -BodyParameter $params

```