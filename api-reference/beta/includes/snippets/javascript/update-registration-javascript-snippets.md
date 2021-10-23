---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b2fb15f2c611b328e56bee4d745b568f9b694fe9
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561044"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const meetingRegistration = {
  subject: 'Microsoft Ignite: Day 1',
  startDateTime: '2021-11-02T08:00:00-08:00',
  endDateTime: '2021-11-02T15:45:00-08:00',
  speakers: [
    {
      displayName: 'Henry Ross',
      bio: 'Chairman and Chief Executive Officer'
    },
    {
      displayName: 'Fred Ryan',
      bio: 'CVP'
    }
  ]
};

await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/registration')
    .version('beta')
    .update(meetingRegistration);

```