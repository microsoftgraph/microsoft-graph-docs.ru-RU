---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 35da9120a970b9624f09521e2a46ed107157014e18943c63dcfdce9842332fdf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57250942"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerBucketTaskBoardTaskFormat = await client.api('/planner/tasks/{task-id}/bucketTaskBoardFormat')
    .get();

```