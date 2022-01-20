---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5e7b62743eb77a4732645dec8ab409e27b17ce56
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116579"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/appointments/AAMkADKqAAA=')
    .version('beta')
    .delete();

```