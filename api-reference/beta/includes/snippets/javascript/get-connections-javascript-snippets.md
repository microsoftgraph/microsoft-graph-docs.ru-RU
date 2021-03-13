---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3cf226cfe5864d01330f2a3a0aca31940ce11526
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805720"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let connections = await client.api('/external/connections')
    .version('beta')
    .get();

```