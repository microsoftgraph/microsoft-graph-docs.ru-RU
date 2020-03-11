---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0ecd66d5dffcaefc70624f79a4d49153eb078375
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591651"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenIssuancePolicy = {
  definition: [
    "definition-value"
  ],
  displayName: "displayName-value",
  isOrganizationDefault: true
};

let res = await client.api('/policies/tokenIssuancePolicies')
    .version('beta')
    .post(tokenIssuancePolicy);

```