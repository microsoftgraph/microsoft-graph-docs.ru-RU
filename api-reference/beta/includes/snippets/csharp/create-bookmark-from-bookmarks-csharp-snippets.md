---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c67e950177f3cb5285eaeca8e623dc2c1f908187
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719757"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookmark = new Microsoft.Graph.Search.Bookmark
{
    DisplayName = "Contoso Install Site",
    WebUrl = "http://www.contoso.com/",
    Description = "Try or buy Contoso for Home or Business and view product information",
    Keywords = new Microsoft.Graph.Search.AnswerKeyword
    {
        Keywords = new List<String>()
        {
            "Contoso",
            "install"
        },
        ReservedKeywords = new List<String>()
        {
            "Contoso"
        },
        MatchSimilarKeywords = true
    },
    AvailabilityStartDateTime = null,
    AvailabilityEndDateTime = null,
    Platforms = new List<DevicePlatformType>()
    {
        DevicePlatformType.Android
    },
    TargetedVariations = new List<Microsoft.Graph.Search.AnswerVariant>()
    {
        new Microsoft.Graph.Search.AnswerVariant
        {
            LanguageTag = "es-es",
            DisplayName = "Sitio de instalación Contoso",
            Description = "Pruebe o compre Contoso hogar o negocios y vea la información del producto"
        }
    },
    State = Microsoft.Graph.Search.AnswerState.Published
};

await graphClient.Search.Bookmarks
    .Request()
    .AddAsync(bookmark);

```