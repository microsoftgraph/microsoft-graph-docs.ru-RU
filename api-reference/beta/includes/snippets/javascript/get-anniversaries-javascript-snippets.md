---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6aeb49959afce9daeb24695bee9257b87df758e9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801740"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let anniversaries = await client.api('/me/profile/anniversaries')
    .version('beta')
    .get();

```