---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3224def202af0faced2de022fa22a1e6b001560b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788491"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerPlanDetails = await client.api('/planner/plans/{plan-id}/details')
    .get();

```