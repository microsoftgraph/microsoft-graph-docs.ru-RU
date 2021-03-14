---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5f74e83e931d29e09ef4890c0ee772da3de27e43
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809833"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messageRules = await client.api('/me/mailFolders/inbox/messageRules')
    .get();

```