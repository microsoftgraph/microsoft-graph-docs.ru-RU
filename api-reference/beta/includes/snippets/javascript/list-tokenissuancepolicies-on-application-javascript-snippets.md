---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ba7337d90acffcb936be14211c8b638850877ea9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797339"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenIssuancePolicies = await client.api('/applications/{id}/tokenIssuancePolicies')
    .version('beta')
    .get();

```