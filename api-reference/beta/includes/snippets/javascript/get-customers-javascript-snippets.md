---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0be75cfcd4f1ee9a3b1329581489cfcef25ac1ad
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790013"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let customers = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers')
    .version('beta')
    .get();

```