---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 110c099c7bbf2bf7c8b0b2914f1c1e08373011fd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798821"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKey = {
  key: 'key-value'
};

await client.api('/trustFramework/keySets/{id}/uploadCertificate')
    .version('beta')
    .post(trustFrameworkKey);

```