---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f1f74bb1d699e2cd1c4d49f29dfe1c12cad53c2ace3ac555abf93f2dfbefebe0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57191504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: 'message-value'
};

await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve')
    .post(approve);

```