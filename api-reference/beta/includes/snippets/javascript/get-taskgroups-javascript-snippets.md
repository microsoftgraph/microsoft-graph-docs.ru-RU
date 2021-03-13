---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ec189faddfd1bce57b31440088b2f191526b4868
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784941"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let taskGroups = await client.api('/me/outlook/taskGroups')
    .version('beta')
    .get();

```