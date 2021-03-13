---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 589bb3f63e812ee92bf9197112b492e8ef796633
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774280"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drive/items/{bundle-id}')
    .version('beta')
    .delete();

```