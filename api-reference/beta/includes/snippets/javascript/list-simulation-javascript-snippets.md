---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3b4f2758b5f4fd343128ebf09a8426bef1e97d9c
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995997"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let simulations = await client.api('/security/attackSimulation/simulations')
    .version('beta')
    .get();

```