---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3b15586ab090cab0c186b4ed8bb3ed8328abf0ea
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638528"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  description: "Group with designated owner and members",
  displayName: "Operations group",
  groupTypes: [
    "Unified"
  ],
  mailEnabled: true,
  mailNickname: "operations2019",
  securityEnabled: false,
  owners@odata.bind: [
    "https://graph.microsoft.com/v1.0/users/26be1845-4119-4801-a799-aea79d09f1a2"
  ],
  members@odata.bind: [
    "https://graph.microsoft.com/v1.0/users/ff7cb387-6688-423c-8188-3da9532a73cc",
    "https://graph.microsoft.com/v1.0/users/69456242-0067-49d3-ba96-9de6f2728e14"
  ]
};

let res = await client.api('/groups')
    .post(group);

```