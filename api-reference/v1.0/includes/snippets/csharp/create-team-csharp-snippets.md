---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8054ff455e40ddf31db2133589f777b5418b8a13
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932560"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    MemberSettings = new TeamMemberSettings
    {
        AllowCreateUpdateChannels = true
    },
    MessagingSettings = new TeamMessagingSettings
    {
        AllowUserEditMessages = true,
        AllowUserDeleteMessages = true
    },
    FunSettings = new TeamFunSettings
    {
        AllowGiphy = true,
        GiphyContentRating = GiphyRatingType.Strict
    }
};

await graphClient.Groups["{id}"].Team
    .Request()
    .PutAsync(team);

```