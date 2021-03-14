---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 68dc5cfa32a5ba43d773aefb495bdcecb221abc1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793654"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscription = await client.api('/me/drive/root/subscriptions/socketIo')
    .get();

```