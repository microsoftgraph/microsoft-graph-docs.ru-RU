---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4da5dfeb1391d068a64077ce9cb2b07da82fefc477ac653b33ee2ce6e3553a2e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57259662"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/oauth2PermissionGrants/{id}')
    .version('beta')
    .delete();

```