---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b2606c6b2c437b4473da062e4dae24690d90c2a9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439283"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  accountEnabled: true,
  displayName: "displayName-value",
  mailNickname: "mailNickname-value",
  userPrincipalName: "upn-value@tenant-value.onmicrosoft.com",
  "passwordProfile" : {
    forceChangePasswordNextSignIn: true,
    password: "password-value"
  }
};

let res = await client.api('/users')
    .version('beta')
    .post({user : user});

```