---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6010dcba86224473906635da661e7ff93a2d5721
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931659"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  recipients: [
    {
      email: "john@contoso.com"
    },
    {
      email: "ryan@external.com"
    }
  ],
  roles: ["read"]
};

let res = await client.api('/shares/{encoded-sharing-url}/permission/grant')
    .version('beta')
    .post(permission);

```