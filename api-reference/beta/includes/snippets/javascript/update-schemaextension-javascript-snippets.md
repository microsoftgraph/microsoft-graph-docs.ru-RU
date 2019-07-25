---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ae6b94e1f8ac311d2af84daa9d46f8d77e0a65c8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718006"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schemaExtension = {
  properties: [
    {
      name:"new-name-value",
      type:"new-type-value"
    },
    {
      name:"additional-name-value",
      type:"additional-type-value"
    }
  ],
};

let res = await client.api('/schemaExtensions/{id}')
    .version('beta')
    .update({schemaExtension : schemaExtension});

```