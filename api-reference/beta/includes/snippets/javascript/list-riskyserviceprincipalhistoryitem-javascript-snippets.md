---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6c5cc277b8d2cb46391f18ded2b78380197f0791
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334606"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let history = await client.api('/identityProtection/riskyServicePrincipals/{riskyServicePrincipalId}/history')
    .version('beta')
    .get();

```