---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6872650023228bb3c66e652cd6678d076a4989e2
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638460"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schemaExtension = {
    id:"graphlearn_courses",
    description: "Graph Learn training courses extensions",
    targetTypes: [
        "Group"
    ],
    properties: [
        {
            name: "courseId",
            type: "Integer"
        },
        {
            name: "courseName",
            type: "String"
        },
        {
            name: "courseType",
            type: "String"
        }
    ]
};

let res = await client.api('/schemaExtensions')
    .post(schemaExtension);

```