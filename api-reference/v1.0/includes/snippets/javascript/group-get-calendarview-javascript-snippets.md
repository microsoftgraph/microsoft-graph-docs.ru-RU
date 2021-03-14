---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c9d26b7f1301dd2b7094da26304183d469398285
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786349"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarView = await client.api('/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-10-01T19:00:00.00-08:00')
    .header('Prefer','outlook.body-content-type="text"')
    .get();

```