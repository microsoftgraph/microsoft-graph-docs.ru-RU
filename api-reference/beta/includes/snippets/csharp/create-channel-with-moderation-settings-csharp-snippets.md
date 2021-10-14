---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 269599fab82ae1f9998321c003980a938adc20e9e40aef67e090573b39e57ec7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57256452"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    DisplayName = "TestChannelModeration",
    Description = "Test channel moderation.",
    MembershipType = ChannelMembershipType.Standard,
    ModerationSettings = new ChannelModerationSettings
    {
        UserNewMessageRestriction = UserNewMessageRestriction.EveryoneExceptGuests,
        ReplyRestriction = ReplyRestriction.Everyone,
        AllowNewMessageFromBots = true,
        AllowNewMessageFromConnectors = true
    }
};

await graphClient.Teams["{team-id}"].Channels
    .Request()
    .AddAsync(channel);

```