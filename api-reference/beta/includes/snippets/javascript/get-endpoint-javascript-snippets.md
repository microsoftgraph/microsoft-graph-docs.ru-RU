---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6330634ed1a2dcd409599543a71fd5eaa0745923
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799954"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let endpoint = await client.api('/groups/{id}/endpoints/{id}')
    .version('beta')
    .get();

```