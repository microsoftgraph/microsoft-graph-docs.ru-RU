---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3440422a276b329cb4a8762b2a8a47e4c03a8f5e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807045"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerTaskDetails = await client.api('/planner/tasks/{task-id}/details')
    .get();

```