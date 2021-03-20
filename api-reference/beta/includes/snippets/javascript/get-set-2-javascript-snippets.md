---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 488bb0f9d7bda5bd2d49cc979ae385a58615b493
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955416"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let set = await client.api('/termStore/sets/{setId}')
    .version('beta')
    .get();

```