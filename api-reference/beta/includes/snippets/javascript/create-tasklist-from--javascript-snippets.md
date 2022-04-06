---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 95441d9973b594ced7437b1b92465d46d1aa2f02
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528772"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const baseTaskList = {
    '@odata.type': '#microsoft.graph.taskList',
    displayName: 'Shopping list'
};

await client.api('/me/tasks/lists')
    .version('beta')
    .post(baseTaskList);

```