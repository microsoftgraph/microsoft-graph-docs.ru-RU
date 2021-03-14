---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2e1efdca031f4653b836ff0fc9b213a53a6e7d81
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789329"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/planner/plans/{plan-id}/tasks')
    .get();

```