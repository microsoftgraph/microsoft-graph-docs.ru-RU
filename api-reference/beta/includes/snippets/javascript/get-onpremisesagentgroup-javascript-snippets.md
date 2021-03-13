---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a57102bfc22b33a220610d670d2bdc17f29ca582
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804497"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let onPremisesAgentGroup = await client.api('/onPremisesPublishingProfiles/provisioning/agentGroups/2d55ed41-1619-4848-92bb-0576d3038682/')
    .version('beta')
    .expand('agents')
    .get();

```