---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 42031a61972d9485dccf071a6ed24a48c74fce2b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787425"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion')
    .version('beta')
    .post();

```