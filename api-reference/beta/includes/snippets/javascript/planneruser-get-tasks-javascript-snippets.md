---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a359255d01bccc4b4ec5d89283a07edfd6f4ea57
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785246"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/me/planner/tasks')
    .version('beta')
    .get();

```