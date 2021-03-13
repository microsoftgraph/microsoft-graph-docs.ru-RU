---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b8f36492da37bb5d8745959d1afddd5419fe092e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791433"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permission = new Permission
{
    Roles = new List<String>()
    {
        "read"
    }
};

await graphClient.Sites["{site-id}"].Permissions["{permission-id}"]
    .Request()
    .UpdateAsync(permission);

```