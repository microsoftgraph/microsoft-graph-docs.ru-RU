---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 210e402cfc4b97a03e44ec48e99a7ea4c787d224
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35505465"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
  directorySetting: {
    displayName: "displayName-value",
    templateId: "templateId-value",
    values: [
      {
        name: "name-value",
        value: "value-value"
      }
    ]
  }
};

let res = await client.api('/groups/{id}/settings')
    .version('beta')
    .post({directorySetting : directorySetting});

```