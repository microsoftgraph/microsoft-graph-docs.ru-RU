---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 446adbb9c41cddbd2826497c63f33c3b5e65ee1d
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514116"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenantAppManagementPolicy = await client.api('/policies/defaultAppManagementPolicy')
    .version('beta')
    .get();

```