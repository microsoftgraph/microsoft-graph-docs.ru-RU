---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 87d2a8bde5b39c4ca38c22d31752e31dcbdd07ca
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789194"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const phoneAuthenticationMethod = {
  phoneNumber: '+1 2065555555',
  phoneType: 'mobile'
};

await client.api('/me/authentication/phoneMethods')
    .version('beta')
    .post(phoneAuthenticationMethod);

```