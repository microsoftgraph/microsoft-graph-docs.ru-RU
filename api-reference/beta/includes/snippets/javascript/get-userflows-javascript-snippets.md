---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0b69fb5a74ce000a913821b038da231bfbc78fe5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793502"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userFlows = await client.api('/identity/userFlows')
    .version('beta')
    .get();

```