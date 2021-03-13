---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 945f18eadff23e15c0c6555f26ab7694fb00ac2a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789692"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlowAttribute = {
  displayName: 'Hobby',
  description: 'Your hobby',
  dataType: 'string',
};

await client.api('/identity/userFlowAttributes')
    .version('beta')
    .post(identityUserFlowAttribute);

```