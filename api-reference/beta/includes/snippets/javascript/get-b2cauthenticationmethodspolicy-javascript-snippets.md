---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 77433e251ad9bde16dc30222b12e7bbcfa58151e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797359"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let b2cAuthenticationMethodsPolicy = await client.api('/policies/b2cAuthenticationMethodsPolicy')
    .version('beta')
    .get();

```