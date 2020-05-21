---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 78225d85d522af7910cb683fcec85d58caf07fa6
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335399"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/oauth2PermissionGrants/{id}')
    .get();

```