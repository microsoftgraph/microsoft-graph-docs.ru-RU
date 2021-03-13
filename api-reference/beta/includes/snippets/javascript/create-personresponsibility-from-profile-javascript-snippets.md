---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 22b3210a22889fe60f333ad9c2c287760fdf4140
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799842"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  description: 'Member of the Microsoft API Council',
  displayName: 'API Council',
  collaborationTags: [
    'askMeAbout'
  ]
};

await client.api('/me/responsibilities')
    .version('beta')
    .post(string);

```