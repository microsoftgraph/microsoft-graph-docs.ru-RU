---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7be7ff80344a98b5c5bcd4240c38d7631c6e6a94
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806805"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  accountEnabled: true,
  displayName: 'Adele Vance',
  mailNickname: 'AdeleV',
  userPrincipalName: 'AdeleV@contoso.onmicrosoft.com',
  passwordProfile: {
    forceChangePasswordNextSignIn: true,
    password: 'xWwvJ]6NMw+bWH-d'
  }
};

await client.api('/users')
    .version('beta')
    .post(user);

```