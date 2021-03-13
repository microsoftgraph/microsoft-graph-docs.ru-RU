---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1524d024b224ced14431d433e03a26fe0cf5130d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778026"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let administrativeUnits = await client.api('/administrativeUnits')
    .version('beta')
    .get();

```