---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7892a531c4d4551beb4910d1efcf5facd681bfdd
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870805"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const swapShiftsChangeRequests = {
  recipientShiftId: "recipientShiftId-value"
};

let res = await client.api('/teams/{id}/schedule/swapShiftsChangeRequests')
    .version('beta')
    .update(swapShiftsChangeRequests);

```