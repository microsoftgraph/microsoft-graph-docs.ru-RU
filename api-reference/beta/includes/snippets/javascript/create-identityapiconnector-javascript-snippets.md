---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 14d853b54e26a7e652d653fed6d9f7aca35ff54c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779989"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
    displayName: 'Test API',
    targetUrl: 'https://someapi.com/api',
    authenticationConfiguration: {
      '@odata.type':'#microsoft.graph.basicAuthentication',
      username: '<USERNAME>',
      password: '<PASSWORD>'
    }
};

await client.api('/identity/apiConnectors')
    .version('beta')
    .post(identityApiConnector);

```