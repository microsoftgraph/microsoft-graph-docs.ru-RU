---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3c88c2f382453c97ae93c2c80ae34d21c59c1337
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777921"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    IsMembershipLimitedToOwners = true,
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
    },
    DiscoverySettings = new TeamDiscoverySettings
    {
        ShowInTeamsSearchAndSuggestions = true
    }
};

await graphClient.Teams["{team-id}"]
    .Request()
    .UpdateAsync(team);

```