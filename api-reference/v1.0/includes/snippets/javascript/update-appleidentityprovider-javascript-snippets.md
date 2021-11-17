---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4516f75c2ac3f306696b8a2aabbcd126ce85b364
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61030844"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviderBase = {
  displayName: 'Apple'
};

await client.api('/identity/identityProviders/Apple-Managed-OIDC')
    .update(identityProviderBase);

```