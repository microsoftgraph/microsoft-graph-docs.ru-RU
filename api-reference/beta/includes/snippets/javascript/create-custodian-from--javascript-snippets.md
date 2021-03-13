---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7aed95129861fccab402cfc4ba1c6d9047c025c0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788075"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const custodian = {
    email: 'AdeleV@contoso.com',
    applyHoldToSources: 'true'
};

await client.api('/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians')
    .version('beta')
    .post(custodian);

```