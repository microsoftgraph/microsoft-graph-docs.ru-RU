---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2f165913afdb9f59cdb7f6f77fbe8edaef2f60b4eafb0dd8cd9906f39f6c5353
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57054898"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const addKey = {
    keyCredential: {
        type: 'AsymmetricX509Cert',
        usage: 'Verify',
        key: 'MIIDYDCCAki...'
    },
    passwordCredential: null,
    proof: 'eyJ0eXAiOiJ...'
};

await client.api('/servicePrincipals/{id}/addKey')
    .version('beta')
    .post(addKey);

```