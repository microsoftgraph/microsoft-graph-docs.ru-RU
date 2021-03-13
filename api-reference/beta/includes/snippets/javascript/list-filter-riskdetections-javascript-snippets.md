---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b3d29b980e389c63cb136ad75bb156022c49cb4c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780395"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskDetections = await client.api('/identityProtection/riskDetections')
    .version('beta')
    .filter('riskEventType eq \'unfamiliarFeatures\' or riskLevel eq \'medium\'')
    .get();

```