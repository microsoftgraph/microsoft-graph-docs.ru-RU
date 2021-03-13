---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9c58f4c4fa405d6eccf3f6712ea9b86f724a7037
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791739"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTask = {
  subject: 'Shop for children\'s weekend',
  startDateTime: {
      dateTime: '2016-05-03T09:00:00',
      timeZone: 'Eastern Standard Time'
  },
  dueDateTime: {
      dateTime: '2016-05-05T16:00:00',
      timeZone: 'Eastern Standard Time'
  }
};

await client.api('/me/outlook/tasks')
    .version('beta')
    .post(outlookTask);

```