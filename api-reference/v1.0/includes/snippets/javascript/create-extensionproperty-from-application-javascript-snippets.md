---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 813f70bfde37491bb3b34dfe2ba57aca4661c5c0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779693"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extensionProperty = {
    name: 'extensionName',
    dataType: 'string',
    targetObjects: [
        'Application'
    ]
};

await client.api('/applications/{id}/extensionProperties')
    .post(extensionProperty);

```