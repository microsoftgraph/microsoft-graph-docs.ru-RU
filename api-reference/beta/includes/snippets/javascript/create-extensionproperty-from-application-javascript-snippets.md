---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 37197f7ba95068d1d5d1c6712e7b27871ba729d2
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995438"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const extensionProperty = {
    name: "extensionName",
    dataType: "string",
    targetObjects: [
        "Application"
    ]
};

let res = await client.api('/applications/{id}/extensionProperties')
    .version('beta')
    .post(extensionProperty);

```