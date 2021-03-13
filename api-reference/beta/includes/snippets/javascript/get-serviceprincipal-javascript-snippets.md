---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 86f1b52f8d578a7591af92209876c8792feef843
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805412"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipal = await client.api('/servicePrincipals/{id}')
    .version('beta')
    .get();

```