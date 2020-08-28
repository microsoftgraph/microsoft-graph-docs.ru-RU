---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 06637bff5409ef6d1b3e9a3dd9bec3ad4b4f3d8f
ms.sourcegitcommit: c4366ac71cf496242c8ff435bc8d8b3816bdc1aa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2020
ms.locfileid: "47287648"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  template@odata.bind: "https://graph.microsoft.com/beta/teamsTemplates('standard')",
  displayName: "My Sample Team",
  description: "My Sample Team’s Description",
  members@odata.bind: [
            {
            @odata.type: "#microsoft.graph.aadUserConversationMember",
            roles: ["owner"],
            userId: "0040b377-61d8-43db-94f5-81374122dc7e"
        }
  ]
};

let res = await client.api('/teams')
    .version('beta')
    .post(team);

```