---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b490690961087d6c8ba4d56b38028c4c6b6992ee
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58369175"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviderBase = {
  '@odata.type': '#microsoft.graph.socialIdentityProvider',
  clientSecret: '1111111111111'
};

await client.api('/identity/identityProviders/Amazon-OAUTH')
    .update(identityProviderBase);

```