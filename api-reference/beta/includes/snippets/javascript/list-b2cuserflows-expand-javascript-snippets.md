---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a246966458ae0caae7464d51a64b88df62e94335
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788621"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2cUserFlows = await client.api('/identity/b2cUserFlows')
    .version('beta')
    .expand('identityProviders')
    .get();

```