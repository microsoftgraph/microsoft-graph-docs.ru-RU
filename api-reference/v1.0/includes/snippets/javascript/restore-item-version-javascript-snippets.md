---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8f66a1bfa806c2df55a8c4dd785a84be82307384
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782995"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/drives/{drive-id}/items/{item-id}/versions/{version-id}/restoreVersion')
    .post();

```