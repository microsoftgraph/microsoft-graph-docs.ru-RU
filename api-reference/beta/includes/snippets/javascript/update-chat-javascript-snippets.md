---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9424006ac0b656b1f7bd9ab052537a7551dc895c
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/13/2021
ms.locfileid: "49845926"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chat = {
    topic: "Group chat title update"
};

let res = await client.api('/chats/19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2')
    .version('beta')
    .update(chat);

```