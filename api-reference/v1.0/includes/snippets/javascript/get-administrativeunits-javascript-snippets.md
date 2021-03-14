---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 80f4b23f061d7164c9541b4b57e25da525947dfe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800726"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let administrativeUnits = await client.api('/directory/administrativeUnits')
    .get();

```