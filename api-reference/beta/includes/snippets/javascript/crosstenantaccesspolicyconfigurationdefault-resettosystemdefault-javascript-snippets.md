---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 36329004b274824586fd82fb00234da526047a20
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336433"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/crossTenantAccessPolicy/default/resetToSystemDefault')
    .version('beta')
    .post();

```