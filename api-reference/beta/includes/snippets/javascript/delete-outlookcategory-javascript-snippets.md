---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a0b80e6b7fbb6a8156377ad9e668d23d5a84a43d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797878"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/outlook/masterCategories/4b1c2495-54c9-4a5e-90a2-0ab0b31987d8')
    .version('beta')
    .delete();

```