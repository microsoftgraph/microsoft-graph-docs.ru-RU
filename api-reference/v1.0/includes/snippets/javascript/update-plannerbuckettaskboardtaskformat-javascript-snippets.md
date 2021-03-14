---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: deae1dfcea4e40456dcd017ae5797229bf07f4d5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790497"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucketTaskBoardTaskFormat = {
  orderHint: 'A6673H Ejkl!'
};

await client.api('/planner/tasks/{task-id}/bucketTaskBoardFormat')
    .update(plannerBucketTaskBoardTaskFormat);

```