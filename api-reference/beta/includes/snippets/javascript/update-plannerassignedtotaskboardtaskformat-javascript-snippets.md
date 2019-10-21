---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 76e7112d21e0a190a3b2ef29979ce035c16c316b
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2019
ms.locfileid: "36638339"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerAssignedToTaskBoardTaskFormat = {
  orderHintsByAssignee: {
    aaa27244-1db4-476a-a5cb-004607466324: "8566473P 957764Jk!"
  }
};

let res = await client.api('/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat')
    .version('beta')
    .update(plannerAssignedToTaskBoardTaskFormat);

```