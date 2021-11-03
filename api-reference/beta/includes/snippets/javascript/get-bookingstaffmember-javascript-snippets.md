---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9093c35993ef0cdf0f27af068fc29926064bd3ff3814c0d50e3a005ad1209857
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141134"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let bookingStaffMember = await client.api('/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/71d64d0e-7225-49b6-b0b1-070d476cda51')
    .version('beta')
    .get();

```