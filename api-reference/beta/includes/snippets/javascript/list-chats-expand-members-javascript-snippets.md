---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 01339641e29d46faa05fc9fbee7a37ca7dd988d9
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5/chats')
    .version('beta')
    .expand('members')
    .get();

```