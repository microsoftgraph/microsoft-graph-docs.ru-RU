---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 848022f3acb4d9d18c4cff5e49950159036a1f98
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204113"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delegatedAdminRelationshipOperation = await client.api('/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836/operations/57e4479a-aafb-4d00-ab0f-8ce6027466cf')
    .version('beta')
    .get();

```