---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 11189adfc8019a58fa54b6d8763beb5117152bb3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938208"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKey = {
  key: "Base64-encoded-pfx-content",
  password: "password-value"
};

let res = await client.api('/trustFramework/keySets/{id}/uploadPkcs12')
    .version('beta')
    .post(trustFrameworkKey);

```