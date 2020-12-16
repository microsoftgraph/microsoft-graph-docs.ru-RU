---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1bd025bbe7c1f1b9e74ef89f541e89e95680941e
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689228"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttributeAssignment = {
  userInputType: "textBox"
};

let res = await client.api('/identity/b2cUserFlows/{b2cIdentityUserFlowId}/userAttributeAssignments/{id}')
    .version('beta')
    .update(identityUserFlowAttributeAssignment);

```