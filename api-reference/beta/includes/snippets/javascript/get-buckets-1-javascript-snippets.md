---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ccc793d4cdbf9f841fc2701c3588fd5908d4bea2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962918"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let buckets = await client.api('/planner/buckets')
    .version('beta')
    .get();

```