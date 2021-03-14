---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 460234d063ff794f2a708ffdfbfda42658dcc5ef
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791843"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  isRead: true,
};

await client.api('/me/messages/{id}')
    .update(message);

```