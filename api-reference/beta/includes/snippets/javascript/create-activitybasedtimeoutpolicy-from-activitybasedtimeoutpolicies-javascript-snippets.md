---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b76e01a6dd7fc421fbf853e16875a0c36a460171
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589960"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const activityBasedTimeoutPolicy = {
  definition: [
    "definition-value"
  ],
  displayName: "displayName-value",
  isOrganizationDefault: true
};

let res = await client.api('/policies/activityBasedTimeoutPolicies')
    .version('beta')
    .post(activityBasedTimeoutPolicy);

```