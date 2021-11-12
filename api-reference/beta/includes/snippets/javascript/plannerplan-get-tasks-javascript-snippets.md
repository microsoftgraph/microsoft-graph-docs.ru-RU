---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8ff268b3f5ba21cf2c275330d6e8fe2e1c458b8ec36259411d672bfa9635c9d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57209918"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/tasks')
    .version('beta')
    .get();

```