---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 613d7f393972420b7e3f1a3f26f3278c6ac1a810
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797106"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenIssuancePolicy = {
  definition: [
    'definition-value'
  ],
  displayName: 'displayName-value',
  isOrganizationDefault: true
};

await client.api('/policies/tokenIssuancePolicies')
    .version('beta')
    .post(tokenIssuancePolicy);

```