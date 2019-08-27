---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: efac581e20c6ec06674dcd22b8ce5a1b0f2eadd5
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638354"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onPremisesAgentGroup = {
    displayName: "Group New Name"
};

let res = await client.api('/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/')
    .version('beta')
    .update(onPremisesAgentGroup);

```