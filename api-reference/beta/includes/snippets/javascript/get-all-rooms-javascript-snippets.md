---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8ac01ed9fac5b753440f8d20d9cff494be7ceeb0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805929"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let room = await client.api('/places/microsoft.graph.room')
    .version('beta')
    .get();

```