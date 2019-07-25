---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 268b8c52bab21f2f238d0d4ceb8c3af54d996e58
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708765"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/unmute')
    .version('beta')
    .post(CommsOperation);

```