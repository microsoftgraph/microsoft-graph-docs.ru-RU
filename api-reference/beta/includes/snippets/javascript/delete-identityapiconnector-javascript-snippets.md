---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0b4c90d9d0fe8b7cf3dae0cd997eaaf80fe52507
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793808"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/apiConnectors/{id}')
    .version('beta')
    .delete();

```