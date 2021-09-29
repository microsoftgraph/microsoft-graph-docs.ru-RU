---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: aa87ab0ef7c95454ab51b20c87b4f6c931299a9b
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996691"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let simulationUsers = await client.api('/security/attackSimulation/simulations/{id}/report/simulationUsers')
    .version('beta')
    .get();

```