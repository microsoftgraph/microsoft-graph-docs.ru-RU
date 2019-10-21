---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e6bfdae9dfe0d224ce669d561fcdf25899f3bcaa
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2019
ms.locfileid: "36638341"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucket = {
  name: "Advertising",
  planId: "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  orderHint: " !"
};

let res = await client.api('/planner/buckets')
    .version('beta')
    .post(plannerBucket);

```