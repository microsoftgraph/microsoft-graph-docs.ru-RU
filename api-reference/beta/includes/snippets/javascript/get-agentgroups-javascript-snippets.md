---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2ea94ad7be72e52603b31d654d29f410fc9baee0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789412"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agentGroups = await client.api('/onPremisesPublishingProfiles/provisioning/agentGroups')
    .version('beta')
    .expand('publishedResources')
    .get();

```