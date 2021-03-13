---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 023d709df36670617d7a87be562fd6b967db3e76
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806178"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userFlowAttributes = await client.api('/identity/userFlowAttributes')
    .version('beta')
    .get();

```