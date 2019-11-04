---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 38357ed43ad6626278fe3b7b1963e2249c156c8d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938575"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlow = {
  userFlowType: "signUpOrSignIn",
  userFlowTypeVersion: 1
};

let res = await client.api('/identity/userFlows')
    .version('beta')
    .post(identityUserFlow);

```