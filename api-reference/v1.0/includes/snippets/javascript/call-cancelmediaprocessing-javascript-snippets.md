---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d5525a3be17fb114a5860193c8265fcb68432cd1
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330125"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancelMediaProcessingOperation = {
  clientContext: "clientContext-value"
};

let res = await client.api('/communications/calls/{id}/cancelMediaProcessing')
    .post(cancelMediaProcessingOperation);

```