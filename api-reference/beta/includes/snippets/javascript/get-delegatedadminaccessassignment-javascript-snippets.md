---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 500fdd9e4f86ae5d0662385c6fd7e181a54ad441
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202575"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delegatedAdminAccessAssignment = await client.api('/tenantRelationships/delegatedAdminRelationships/72a7ae7e-4887-4e34-9755-2e1e9b26b943-63f017cb-9e0d-4f14-94bd-4871902b3409/accessAssignments/da9d6cf90-083a-47dc-ace2-1da98be3f344')
    .version('beta')
    .get();

```