---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7a7d25d353538b847760605ce7f2e4356df9213f
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/15/2019
ms.locfileid: "37995606"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const passwordCredential = {
  passwordCredential: {
    displayName: "Password friendly name"
  }
};

let res = await client.api('/applications/{id}/addPassword')
    .version('beta')
    .post(passwordCredential);

```