---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c630207749b14526bf63b507d0c77e2f4cf03b4a6a26ee55859973987ab301b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57055116"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
    body: {
        contentType: 'html',
        content: '<div><div><at id=\"0\">GraphTesting</at>&nbsp;Hello team</div></div>'
    },
    mentions: [
        {
            id: 0,
            mentionText: 'GraphTesting',
            mentioned: {
                conversation: {
                    id: '68a3e365-f7d9-4a56-b499-24332a9cc572',
                    displayName: 'GraphTesting',
                    conversationIdentityType: 'team'
                }
            }
        }
    ],
    reactions: []
};

await client.api('/teams/68a3e365-f7d9-4a56-b499-24332a9cc572/channels/19:0b50940236084d258c97b21bd01917b0@thread.skype/messages')
    .version('beta')
    .post(chatMessage);

```