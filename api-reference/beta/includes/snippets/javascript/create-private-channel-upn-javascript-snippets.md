---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6cabb48498c5d6432617a8fdfeca7cd4b2a1ad55
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688056"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
  '@odata.type': '#Microsoft.Graph.channel',
  membershipType: 'private',
  displayName: 'My First Private Channel',
  description: 'This is my first private channels',
  members: 
     [
        {
           '@odata.type':'#microsoft.graph.aadUserConversationMember',
           'user@odata.bind':'https://graph.microsoft.com/beta/users(\'jacob@contoso.com\')',
           roles: ['owner']
        }
     ]
};

await client.api('/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels')
    .version('beta')
    .post(channel);

```