---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f723cf755da340dfc59ce5f30f90d7120123132af11c850e021bb8a03cfa7115
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57251709"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let user = await client.api('/users/{id}')
    .version('beta')
    .get();

```