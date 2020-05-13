---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 15cda19c2a35cfc2609081601fadb19238e9e528
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44219299"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: "message-value"
};

let res = await client.api('/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve')
    .version('beta')
    .post(approve);

```