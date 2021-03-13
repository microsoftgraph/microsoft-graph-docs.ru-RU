---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d3477a61e5cf80e974d84ef445b498d31b095f4e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802125"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttributeAssignment = {
  userInputType: 'textBox'
};

await client.api('/identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/{id}')
    .version('beta')
    .update(identityUserFlowAttributeAssignment);

```