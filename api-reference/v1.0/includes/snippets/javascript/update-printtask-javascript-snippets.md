---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2eadbb5de0df7de39cc3addaaa5aab41f9eb50dd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771318"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printTask = {
  status: {
    state: 'completed',
    description: 'completed'
  }
};

await client.api('/print/taskDefinitions/{taskDefinitionId}/tasks/{taskId}')
    .update(printTask);

```