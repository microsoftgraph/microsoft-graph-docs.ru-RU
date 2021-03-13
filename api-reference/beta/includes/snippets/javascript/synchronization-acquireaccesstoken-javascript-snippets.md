---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a017ea179aa4a2192fe5ea23feff2fc54f67d0ce
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794692"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const acquireAccessToken = {
  credentials: [
    {
      '@odata.type': 'microsoft.graph.synchronizationSecretKeyStringValuePair'
    }
  ]
};

await client.api('/applications/{applicationsId}/synchronization/acquireAccessToken')
    .version('beta')
    .post(acquireAccessToken);

```