---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ca6fda7e9c64c0896af45710497c32d323be51a7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810160"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/me')
    .version('beta')
    .get();

```