---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 54c7b2cdbe5932197d87e2d621dadf1c7617ded1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792104"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let riskyUsers = await client.api('/identityProtection/riskyUsers')
    .version('beta')
    .filter('riskLevel eq microsoft.graph.riskLevel\'medium\'')
    .get();

```