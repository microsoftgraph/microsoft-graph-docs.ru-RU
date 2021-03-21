---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cb66dc2637949ef1f0a90a6e4b502748351751fd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963261"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const hybridAgentUpdaterConfiguration = {
    deferUpdate: '2018-08-20T12:00'
};

await client.api('/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration')
    .version('beta')
    .update(hybridAgentUpdaterConfiguration);

```