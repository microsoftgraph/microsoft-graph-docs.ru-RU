---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f67989a23e6dd19d6f82ab1cc69ad5d8e5ea9442
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794359"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let passwordAuthenticationMethod = await client.api('/me/authentication/passwordMethods/{id}')
    .version('beta')
    .get();

```