---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b22748c579e7e47a6f4270d8052acd859539b6d5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783593"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationFlowsPolicy = {
  selfServiceSignUp: {
    isEnabled: true
  }
};

await client.api('/policies/authenticationFlowsPolicy')
    .version('beta')
    .update(authenticationFlowsPolicy);

```