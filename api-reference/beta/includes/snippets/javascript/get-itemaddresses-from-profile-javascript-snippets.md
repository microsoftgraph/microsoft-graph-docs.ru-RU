---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 415361b9dae1eef39a81135faab1f11e7e064082
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let addresses = await client.api('/me/profile/addresses')
    .version('beta')
    .get();

```