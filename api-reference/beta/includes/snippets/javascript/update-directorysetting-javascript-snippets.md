---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2a02ac999b23ffce68347a1d1823af8ba81de32d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706386"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
  values: [
    {
      name: "name-value",
      value: "value-value"
    }
  ]
};

let res = await client.api('/settings/{id}')
    .version('beta')
    .update({directorySetting : directorySetting});

```