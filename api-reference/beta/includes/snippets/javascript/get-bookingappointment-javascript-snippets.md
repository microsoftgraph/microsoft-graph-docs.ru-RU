---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e929c49232ac61fc92d3341a7975102fa21d7973
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801511"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingAppointment = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=')
    .version('beta')
    .get();

```