---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5444b6bf58454917e84d80714421e2eea44bfedf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  metadata: "metadata-value",
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/updateMetadata')
    .version('beta')
    .post(CommsOperation);

```