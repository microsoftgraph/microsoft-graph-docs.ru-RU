---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4d62dd721e27743ed613f2f880d617355b49619b7168fcccb204d6b3d7835d14
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57396227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
    'template@odata.bind': 'https://graph.microsoft.com/beta/teamsTemplates(\'standard\')',
    visibility: 'Private',
    displayName: 'Sample Engineering Team',
    description: 'This is a sample engineering team, used to showcase the range of properties supported by this API',
    channels: [
        {
            displayName: 'Announcements 📢',
            isFavoriteByDefault: true,
            description: 'This is a sample announcements channel that is favorited by default. Use this channel to make important team, product, and service announcements.'
        },
        {
            displayName: 'Training 🏋️',
            isFavoriteByDefault: true,
            description: 'This is a sample training channel, that is favorited by default, and contains an example of pinned website and YouTube tabs.',
            tabs: [
                {
                    'teamsApp@odata.bind': 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.web\')',
                    displayName: 'A Pinned Website',
                    configuration: {
                        contentUrl: 'https://docs.microsoft.com/microsoftteams/microsoft-teams'
                    }
                },
                {
                    'teamsApp@odata.bind': 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.youtube\')',
                    displayName: 'A Pinned YouTube Video',
                    configuration: {
                        contentUrl: 'https://tabs.teams.microsoft.com/Youtube/Home/YoutubeTab?videoId=X8krAMdGvCQ',
                        websiteUrl: 'https://www.youtube.com/watch?v=X8krAMdGvCQ'
                    }
                }
            ]
        },
        {
            displayName: 'Planning 📅 ',
            description: 'This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.',
            isFavoriteByDefault: false
        },
        {
            displayName: 'Issues and Feedback 🐞',
            description: 'This is a sample of a channel that is not favorited by default, these channels will appear in the more channels overflow menu.'
        }
    ],
    memberSettings: {
        allowCreateUpdateChannels: true,
        allowDeleteChannels: true,
        allowAddRemoveApps: true,
        allowCreateUpdateRemoveTabs: true,
        allowCreateUpdateRemoveConnectors: true
    },
    guestSettings: {
        allowCreateUpdateChannels: false,
        allowDeleteChannels: false
    },
    funSettings: {
        allowGiphy: true,
        giphyContentRating: 'Moderate',
        allowStickersAndMemes: true,
        allowCustomMemes: true
    },
    messagingSettings: {
        allowUserEditMessages: true,
        allowUserDeleteMessages: true,
        allowOwnerDeleteMessages: true,
        allowTeamMentions: true,
        allowChannelMentions: true
    },
    discoverySettings: {
        showInTeamsSearchAndSuggestions: true
    },
    installedApps: [
        {
            'teamsApp@odata.bind': 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.vsts\')'
        },
        {
            'teamsApp@odata.bind': 'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'1542629c-01b3-4a6d-8f76-1938b779e48d\')'
        }
    ]
};

await client.api('/teams')
    .version('beta')
    .post(team);

```