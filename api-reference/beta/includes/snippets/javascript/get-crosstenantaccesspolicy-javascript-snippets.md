---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0ced1b2c2f6fdcf8d3f3bfdde8a4836f9de68a33
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336587"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let crossTenantAccessPolicy = await client.api('/policies/crossTenantAccessPolicy')
    .version('beta')
    .get();

```