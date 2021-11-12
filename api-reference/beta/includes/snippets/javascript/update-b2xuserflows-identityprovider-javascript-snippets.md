---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 201ae6f4963ed1b04ebfe5a686650fbff859e978f48c4a5089e9b02d6043ec9c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57198061"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
  '@odata.id': 'https://graph.microsoft.com/beta/identityProviders/{id}'
};

await client.api('/identity/b2xUserFlows/{id}/identityProviders/$ref')
    .version('beta')
    .post(identityProvider);

```