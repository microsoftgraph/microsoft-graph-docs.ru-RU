---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f046101bd48b2e49f4f8e93abac16eb03bedb176
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713938"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedAccess/azureResources/resources')
    .version('beta')
    .get();

```