---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aeb43b779a6f8c140bc387b670fc8a7077112f54
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805464"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const program = {
    displayName: 'testprogram3',
    description: 'test description'
};

await client.api('/programs')
    .version('beta')
    .post(program);

```