---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6fb36530518c0a3bd20103548d84e5272fd2626a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804064"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/activities/13881113971988980728/')
    .version('beta')
    .delete();

```