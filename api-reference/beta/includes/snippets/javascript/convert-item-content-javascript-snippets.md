---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8b638ee0c80d012fba06b3019551a4bf9a4d1e47
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796012"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/drive/items/{item-id}/content?format=%7Bformat%7D')
    .version('beta')
    .get();

```