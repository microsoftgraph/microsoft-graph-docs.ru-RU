---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0e8b5027f232dac65f9beacf2a9255d9f5c13ec9
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220705"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let signIns = await client.api('/auditLogs/signins')
    .version('beta')
    .filter('startsWith(appDisplayName,\'Azure\')')
    .top(10)
    .get();

```