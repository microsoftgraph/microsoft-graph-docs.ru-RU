---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b07ca951d7d9e1566b1099e76e123b43a9a3af5a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774042"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let defaultPages = await client.api('/identity/b2cUserFlows/B2C_1_Customer/languages/en/defaultPages')
    .version('beta')
    .get();

```