---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 632ae117f5e0fa51e93ac71f02b7aa4bdb4af731
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805318"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviders = {
  '@odata.id': 'https://graph.microsoft.com/beta/identityProviders/{id}'
};

await client.api('/identity/b2cUserFlows/{id}/identityProviders/$ref')
    .version('beta')
    .update(identityProviders);

```