---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 14422b0f3b3474fac579ba8a635b60289a9985bd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788744"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let presence = await client.api('/me/presence')
    .version('beta')
    .get();

```