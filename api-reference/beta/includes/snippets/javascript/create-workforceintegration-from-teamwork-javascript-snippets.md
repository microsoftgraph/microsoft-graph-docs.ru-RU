---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 37cd1529da4d10386ed09b9d715d4632e2be9390
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778621"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workforceIntegration = {
  displayName: 'displayName-value',
  apiVersion: 99,
  encryption: {
    protocol: 'protocol-value',
    secret: 'secret-value'
  },
  isActive: true,
  url: 'url-value',
  supports: 'supports-value'
};

await client.api('/teamwork/workforceIntegrations')
    .version('beta')
    .post(workforceIntegration);

```