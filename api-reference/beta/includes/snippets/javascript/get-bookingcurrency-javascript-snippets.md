---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 01925c6ae736d7abc9961d30be70a5a781eefec6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795511"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingCurrency = await client.api('/bookingCurrencies/USD')
    .version('beta')
    .get();

```