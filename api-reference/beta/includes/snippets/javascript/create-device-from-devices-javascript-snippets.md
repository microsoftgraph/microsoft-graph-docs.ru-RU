---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1e1527773359bfdb32a1049354f5afbb4fd326dd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802823"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const device = {
  accountEnabled: true,
  alternativeSecurityIds: [
    {
      type: 99,
      identityProvider: 'identityProvider-value',
      key: 'base64Y3YxN2E1MWFlYw=='
    }
  ],
  approximateLastSignInDateTime: '2016-10-19T10:37:00Z',
  deviceId: 'deviceId-value',
  deviceMetadata: 'deviceMetadata-value',
  deviceVersion: 99
};

await client.api('/devices')
    .version('beta')
    .post(device);

```