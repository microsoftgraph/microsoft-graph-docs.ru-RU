---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6d27d95b1a69fb6eb03fbf82a40d3e068147d177
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620687"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  destinationId: "deleteditems"
};

let res = await client.api('/me/messages/AAMkADhAAATs28OAAA=/move')
    .version('beta')
    .post(message);

```