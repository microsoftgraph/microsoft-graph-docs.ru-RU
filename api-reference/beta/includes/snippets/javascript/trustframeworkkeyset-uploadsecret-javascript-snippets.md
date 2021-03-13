---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b8698ec35f6f9449d9eb9343c0ef1b9f25f05969
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801998"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKey = {
  use: 'use-value',
  k: 'application-secret-to-be-uploaded',
  nbf: 1508969811,
  exp: 1508973711
};

await client.api('/trustFramework/keySets/{id}/uploadSecret')
    .version('beta')
    .post(trustFrameworkKey);

```