---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 52bb5a9cabfc9a72c49eaccb735d0c82bf65c0ed
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35505466"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
  templateId: "templateId-value",
  values: [
    {
      name: "name-value",
      value: "value-value"
    }
  ]
};

let res = await client.api('/settings')
    .version('beta')
    .post({directorySetting : directorySetting});

```