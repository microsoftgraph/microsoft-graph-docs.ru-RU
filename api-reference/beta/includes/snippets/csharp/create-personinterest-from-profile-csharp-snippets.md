---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 24ae32af5dffee7d2349cd0e2aed66b36064c407
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821338"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personInterest = new PersonInterest
{
    Categories = new List<String>()
    {
        "Sports"
    },
    Description = "World's greatest football club",
    DisplayName = "Chelsea FC",
    WebUrl = "https://www.chelseafc.com"
};

await graphClient.Me.Profile.Interests
    .Request()
    .AddAsync(personInterest);

```