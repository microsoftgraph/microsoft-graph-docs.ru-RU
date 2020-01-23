---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cfd3bf74239a0a5ef2806ee55d88617a4f941305
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476349"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const policy = {
  definition: [
    "definition-value"
  ],
  displayName: "displayName-value",
  isOrganizationDefault: true
};

let res = await client.api('/policies/claimsMappingPolicies')
    .version('beta')
    .post(policy);

```