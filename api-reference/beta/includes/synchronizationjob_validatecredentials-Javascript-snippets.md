---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9bd2d6024438dffb75c384642dd83c8ae9844fce
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465939"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const validateCredentials = {
    credentials: [ 
        { key: "UserName", value: "user@domain.com" },
        { key: "Password", value: "password-value" }
    ]
};

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials')
    .version('beta')
    .post(validateCredentials);

```