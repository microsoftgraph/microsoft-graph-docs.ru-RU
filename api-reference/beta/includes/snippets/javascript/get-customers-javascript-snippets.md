---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 8bde6c2adb74421f22a9de676749f764dcea2bab
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094755"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let customers = await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/customers')
    .version('beta')
    .get();

```