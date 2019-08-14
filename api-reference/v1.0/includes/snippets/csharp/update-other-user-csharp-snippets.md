---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a77b2874d4e70f79d99c00d0a9895bee1bcb4f80
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396837"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = new User
{
    BusinessPhones = new List<String>()
    {
        "businessPhones-value"
    },
    OfficeLocation = "city-value"
};

await graphClient.Users["{id}"]
    .Request()
    .UpdateAsync(user);

```