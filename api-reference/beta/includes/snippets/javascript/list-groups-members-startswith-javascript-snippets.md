---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 80d314a3baccf40d52753ba81f92a1b290ba781b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211673"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/groups/{id}/members')
    .version('beta')
    .header('ConsistencyLevel','eventual')
    .filter('startswith(displayName, \'a\')')
    .get();

```