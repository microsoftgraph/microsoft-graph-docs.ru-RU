---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a2a097a16d707bb79eb4f5261ce17131d2f6eb72
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977479"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = new Team();
team.isMembershipLimitedToOwners = true;
TeamMemberSettings memberSettings = new TeamMemberSettings();
memberSettings.allowCreateUpdateChannels = true;
team.memberSettings = memberSettings;
TeamMessagingSettings messagingSettings = new TeamMessagingSettings();
messagingSettings.allowUserEditMessages = true;
messagingSettings.allowUserDeleteMessages = true;
team.messagingSettings = messagingSettings;
TeamFunSettings funSettings = new TeamFunSettings();
funSettings.allowGiphy = true;
funSettings.giphyContentRating = GiphyRatingType.STRICT;
team.funSettings = funSettings;
TeamDiscoverySettings discoverySettings = new TeamDiscoverySettings();
discoverySettings.showInTeamsSearchAndSuggestions = true;
team.discoverySettings = discoverySettings;

graphClient.teams("{id}")
    .buildRequest()
    .patch(team);

```