---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 66fabd50d75e2d63a622d2ab75e77f5017ae142f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798318"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamsApps = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('distributionMethod eq \'organization\'')
    .get();

```