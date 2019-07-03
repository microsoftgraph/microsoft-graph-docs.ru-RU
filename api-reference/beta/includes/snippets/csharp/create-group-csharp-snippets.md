---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c52999d92ffd7048080e0381185e3a63aec49e2d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35464795"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Self help community for golf",
    DisplayName = "Golf Assist",
    GroupTypes = new List<String>()
    {
        "Unified"
    },
    MailEnabled = true,
    MailNickname = "golfassist",
    SecurityEnabled = false
};

await graphClient.Groups
    .Request()
    .AddAsync(group);

```