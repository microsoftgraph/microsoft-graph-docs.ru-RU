---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2a069a67dd4216c6cc91f9ad2fec0ce8a1eddf304b5437a2f64d5079d7221ba5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57144563"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let outcomes = await client.api('/education/classes/{id}/assignments/{id}/submissions/{id}/outcomes')
    .version('beta')
    .get();

```