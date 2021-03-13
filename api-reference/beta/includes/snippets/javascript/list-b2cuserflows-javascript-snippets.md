---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e5b00d4f6df63d93ff9f067279b3afa5a7e2faed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810244"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2cUserFlows = await client.api('/identity/b2cUserFlows')
    .version('beta')
    .get();

```