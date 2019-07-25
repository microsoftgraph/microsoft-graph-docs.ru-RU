---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 64f3465f2cca9a803587aec82f5a86b32e439e67
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711278"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    AccountEnabled = true,
    BusinessPhones = new List<String>()
    {
        "businessPhones-value"
    },
    City = "city-value"
};

await graphClient.Me
    .Request()
    .UpdateAsync(user);

```