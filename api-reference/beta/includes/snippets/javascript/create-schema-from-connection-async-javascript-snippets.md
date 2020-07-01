---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6f19c86496729c9d4c21d58c43c29e9c106691cc
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/01/2020
ms.locfileid: "45008664"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schema = {
  baseType: "microsoft.graph.externalItem",
  properties: [
    {
      name: "ticketTitle",
      type: "String",
      isSearchable: "true",
      isRetrievable: "true",
      labels: [
        "title"
      ]
    },
    {
      name: "priority",
      type: "String",
      isQueryable: "true",
      isRetrievable: "true",
      isRefinable: "true",
      isSearchable: "false"
    },
    {
      name: "assignee",
      type: "String",
      isRetrievable: "true"
    }
  ]
};

let res = await client.api('/connections/contosohr/schema')
    .version('beta')
    .post(schema);

```