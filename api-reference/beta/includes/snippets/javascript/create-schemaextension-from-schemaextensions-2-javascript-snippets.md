---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4af6c8cb41de589070933d911c3eacbfb60b306a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802593"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schemaExtension = {
    id: 'courses',
    description: 'Graph Learn training courses extensions',
    targetTypes: [
        'Group'
    ],
    properties: [
        {
            name: 'courseId',
            type: 'Integer'
        },
        {
            name: 'courseName',
            type: 'String'
        },
        {
            name: 'courseType',
            type: 'String'
        }
    ]
};

await client.api('/schemaExtensions')
    .version('beta')
    .post(schemaExtension);

```