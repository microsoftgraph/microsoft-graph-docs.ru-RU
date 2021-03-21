---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9d2a06c67bd50c015f65c571d96bc877eca93f21
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962193"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ownedObjects = await client.api('/servicePrincipals/{id}/ownedObjects')
    .version('beta')
    .get();

```