---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1ca4d762dc65e230ea07fff26f2da339ecc2b22f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794349"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb')
    .version('beta')
    .delete();

```