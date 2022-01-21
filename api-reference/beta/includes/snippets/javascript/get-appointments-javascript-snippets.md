---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3b0a48afcf5d942a5339d5fbaddc9d6409ceea55
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62109765"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let appointments = await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments')
    .version('beta')
    .get();

```