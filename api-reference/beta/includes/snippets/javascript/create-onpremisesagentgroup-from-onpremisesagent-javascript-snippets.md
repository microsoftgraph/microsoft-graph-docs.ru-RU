---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 312380021b9793d5ec8e1b24f3b8b949e1cb85e5868aa6cf8aaa1e79bd08118a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57263731"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref')
    .version('beta')
    .post();

```