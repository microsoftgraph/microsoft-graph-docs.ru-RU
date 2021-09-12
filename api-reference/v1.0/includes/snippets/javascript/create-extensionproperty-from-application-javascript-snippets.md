---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fe3795db63983f2c11fea4eb3c7acb44d6f154e8a0d7c45e0795c22f6c7879cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57267352"
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