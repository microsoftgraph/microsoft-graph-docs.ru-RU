---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fcbad503ec8bc7f2881a7688805e26ecf4919265
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937522"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKey = {
  key: "key-value"
};

let res = await client.api('/trustFramework/keySets/{id}/uploadCertificate')
    .version('beta')
    .post(trustFrameworkKey);

```