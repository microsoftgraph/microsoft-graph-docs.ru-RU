---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4aa5ae9ec58f04ddc35cb8b4c8f47f3fc756cf600cab7deae7a303faf84c4f90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052191"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    DisplayName = "My Class Team",
    Description = "My Class Team’s Description",
    Channels = new TeamChannelsCollectionPage()
    {
        new Channel
        {
            DisplayName = "Class Announcements 📢",
            IsFavoriteByDefault = true
        },
        new Channel
        {
            DisplayName = "Homework 🏋️",
            IsFavoriteByDefault = true
        }
    },
    MemberSettings = new TeamMemberSettings
    {
        AllowCreateUpdateChannels = false,
        AllowDeleteChannels = false,
        AllowAddRemoveApps = false,
        AllowCreateUpdateRemoveTabs = false,
        AllowCreateUpdateRemoveConnectors = false
    },
    InstalledApps = new TeamInstalledAppsCollectionPage()
    {
        new TeamsAppInstallation
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"teamsApp@odata.bind", "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('com.microsoft.teamspace.tab.vsts')"}
            }
        },
        new TeamsAppInstallation
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"teamsApp@odata.bind", "https://graph.microsoft.com/v1.0/appCatalogs/teamsApps('1542629c-01b3-4a6d-8f76-1938b779e48d')"}
            }
        }
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind", "https://graph.microsoft.com/v1.0/teamsTemplates('educationClass')"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```