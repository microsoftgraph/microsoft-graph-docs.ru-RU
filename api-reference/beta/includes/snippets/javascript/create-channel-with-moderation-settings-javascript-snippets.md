---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 848d9a8a5b841b238e92a3162559d1ae2f4bcbcc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778487"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
    displayName: 'TestChannelModeration',
    description: 'Test channel moderation.',
    membershipType: 'standard',
    moderationSettings: {
        userNewMessageRestriction: 'everyoneExceptGuests',
        replyRestriction: 'everyone',
        allowNewMessageFromBots: true,
        allowNewMessageFromConnectors: true
    }
};

await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels')
    .version('beta')
    .post(channel);

```