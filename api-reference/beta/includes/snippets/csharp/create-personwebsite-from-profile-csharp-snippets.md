---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 30fd2290f0b925cfbac9c51e3acbbee5586128ee
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821151"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personWebsite = new PersonWebsite
{
    Categories = new List<String>()
    {
        "football"
    },
    DisplayName = "Lyn Damer",
    WebUrl = "www.lyndamer.no"
};

await graphClient.Me.Profile.Websites
    .Request()
    .AddAsync(personWebsite);

```