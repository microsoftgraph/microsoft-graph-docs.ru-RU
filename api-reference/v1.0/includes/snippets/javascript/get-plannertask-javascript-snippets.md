---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 51ba2a2cb15ef8dc5bcabd3283ca3724deca856c9488512e80f24084d1a0998d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57319348"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerTask = await client.api('/planner/tasks/{task-id}')
    .get();

```