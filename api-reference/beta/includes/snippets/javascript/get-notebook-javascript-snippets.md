---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8d33189671111605c4a86a4388286e9117bc8ab6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782933"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let notebook = await client.api('/me/onenote/notebooks/{id}')
    .version('beta')
    .get();

```