---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b8cfc8f52e439e78794092f960455de19a0a96592efadf0e28fd2e0c9cc5f2ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57254326"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let resources = await client.api('/privilegedAccess/azureResources/resources')
    .version('beta')
    .get();

```