---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a5f42f3737a86fca0576f5d4bbe330a8d611694f20eba07d09942c61d5217ffb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57246896"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenant = await client.api('/tenantRelationships/managedTenants/tenants/{tenantId}')
    .version('beta')
    .get();

```