---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 73acbf198aa2cae46e6faf2ebf437f592006aad4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116397"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingStaffMember = await client.api('/bookingBusinesses/Contosolunchdelivery@contoso.onmicrosoft.com/staffmembers/71d64d0e-7225-49b6-b0b1-070d476cda51')
    .version('beta')
    .get();

```