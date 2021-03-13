---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 775df42c21b1feea7ea0152c03f9ec9521413f8b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787426"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let licenseDetails = await client.api('/me/licenseDetails')
    .version('beta')
    .get();

```