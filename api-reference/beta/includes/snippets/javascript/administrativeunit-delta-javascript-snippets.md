---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7090fa47c6d4926da9f855cfc6d93dfeeeac4202
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805761"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/administrativeUnits/delta')
    .version('beta')
    .get();

```