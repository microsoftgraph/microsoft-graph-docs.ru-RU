---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1cf84e91157063bbf1a86f766692e779a2599b98
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638501"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const messageRule = {
    displayName: "Important from partner",
    actions: {
        markImportance: "high"
     }
};

let res = await client.api('/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=')
    .update(messageRule);

```