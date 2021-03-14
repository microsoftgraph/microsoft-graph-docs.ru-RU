---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e248252d52592ba3ceebf4e8c304637a0d517744
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787920"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  destinationId: 'deleteditems'
};

await client.api('/me/messages/AAMkADhAAATs28OAAA=/move')
    .post(message);

```