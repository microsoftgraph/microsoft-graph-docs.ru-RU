---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c5638e0f034877e1a3f753c7fab2d5c253daeb3d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780536"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let programs = await client.api('/programs')
    .version('beta')
    .get();

```