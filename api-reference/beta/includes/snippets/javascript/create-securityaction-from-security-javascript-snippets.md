---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a3f251e232d7e90adccfcf8de82af0538de3c5b4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788371"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const securityAction = {
  name: 'BlockIp',
  actionReason: 'Test',
  parameters: [
    {
      name: 'IP',
      value: '1.2.3.4'
    }
  ],
  vendorInformation: {
    provider: 'Windows Defender ATP',
    vendor: 'Microsoft'
  }
};

await client.api('/security/securityActions')
    .version('beta')
    .post(securityAction);

```