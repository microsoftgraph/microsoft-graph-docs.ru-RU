---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ce3d6b6b0f1a1956e8a3c0cd1f3f2a5df6652c1f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773937"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agreements = await client.api('/identityGovernance/termsOfUse/agreements')
    .version('beta')
    .get();

```