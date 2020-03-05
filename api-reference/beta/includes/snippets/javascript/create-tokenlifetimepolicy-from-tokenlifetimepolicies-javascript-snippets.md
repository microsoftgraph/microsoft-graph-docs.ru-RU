---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2b506cf74a70033cf58e5cbab353ba2a8935b330
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2020
ms.locfileid: "41558900"
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

let res = await client.api('/policies/tokenLifetimePolicies')
    .version('beta')
    .post(policy);

```