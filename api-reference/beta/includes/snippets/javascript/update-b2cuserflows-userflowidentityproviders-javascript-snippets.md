---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6943b52cdf36a640ba9eede195638cad06f69e7b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58369155"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userFlowIdentityProviders = {
  '@odata.id': 'https://graph.microsoft.com/beta/identity/identityProviders/{id}',
  '@odata.type': '#microsoft.graph.identityProvider'
};

await client.api('/identity/b2cUserFlows/B2C_test_signin_signup/userflowIdentityProviders/$ref')
    .version('beta')
    .update(userFlowIdentityProviders);

```