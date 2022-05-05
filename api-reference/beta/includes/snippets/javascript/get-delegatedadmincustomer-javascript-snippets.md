---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f5a8b78f3fefe690bf418418472b9c1ca8c43229
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202614"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delegatedAdminCustomer = await client.api('/tenantRelationships/delegatedAdminCustomers/4fdbff88-9d6b-42e0-9713-45c922ba8001')
    .version('beta')
    .get();

```