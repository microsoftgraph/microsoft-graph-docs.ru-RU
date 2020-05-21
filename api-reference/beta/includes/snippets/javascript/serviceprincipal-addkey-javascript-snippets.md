---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6ef8dadb218d9c94019798bf76d389d459afc797
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333983"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const addKey = {
    keyCredential: {
        type: "X509CertAndPassword",
        usage: "Sign",
        key: "MIIDYDCCAki..."
    },
    passwordCredential: {
        secretText: "MKTr0w1..."
    },
    proof:"eyJ0eXAiOiJ..."
};

let res = await client.api('/serviceprincipals/{id}/addKey')
    .version('beta')
    .post(addKey);

```