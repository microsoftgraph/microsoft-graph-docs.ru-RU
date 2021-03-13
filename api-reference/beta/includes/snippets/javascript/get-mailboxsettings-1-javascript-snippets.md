---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 105f1a28d1a520ef0ad3c2fba157d6c3c95896ab
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778476"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let mailboxSettings = await client.api('/me/mailboxSettings')
    .version('beta')
    .get();

```