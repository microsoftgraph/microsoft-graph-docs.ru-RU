---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 559a6be570b7e25a19051e996c041a0b9e080797
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713910"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedAccess/azureResources/roleAssignmentRequests/7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee/cancel')
    .version('beta')
    .post();

```