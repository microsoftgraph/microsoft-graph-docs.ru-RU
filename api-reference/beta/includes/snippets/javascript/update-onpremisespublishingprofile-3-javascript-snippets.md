---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1f5ff81c3e437d1352180602c774e5aedd84093b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963268"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const hybridAgentUpdaterConfiguration = {
    allowUpdateConfigurationOverride: false
};

await client.api('/onPremisesPublishingProfiles/provisioning/hybridAgentUpdaterConfiguration')
    .version('beta')
    .update(hybridAgentUpdaterConfiguration);

```