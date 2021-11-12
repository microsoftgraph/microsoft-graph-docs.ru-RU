---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f4a41698cf358e66d9e2397fb638143d6d5faf18ddeca9998679e30b1fb5dc5d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57053454"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
  values: [
    {
      name: 'name-value',
      value: 'value-value'
    }
  ]
};

await client.api('/settings/{id}')
    .version('beta')
    .update(directorySetting);

```