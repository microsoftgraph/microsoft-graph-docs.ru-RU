---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fd3f5033adb87620dc7816e8cf8e66c9f3535ff1ad2002bf550568e0b5defec4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57246616"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const keyCredential = {
    keyCredential: {
        type: 'AsymmetricX509Cert',
        usage: 'Verify',
        key: 'MIIDYDCCAki...'
    },
    passwordCredential: null,
    proof: 'eyJ0eXAiOiJ...'
};

await client.api('/applications/{id}/addKey')
    .version('beta')
    .post(keyCredential);

```