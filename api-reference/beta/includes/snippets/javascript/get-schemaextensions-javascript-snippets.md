---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 45912f6ada4ce5a19566689d06e68bde55042e2c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schemaExtensions = await client.api('/schemaExtensions')
    .version('beta')
    .filter('id eq \'graphlearn_test\'')
    .get();

```