---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7d6a94daa6b2331159eaddc326d6893f4c2ec5e9b37c670e9112aa529f1c6239
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57361599"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  originalStartTimeZone: 'originalStartTimeZone-value',
  originalEndTimeZone: 'originalEndTimeZone-value',
  responseStatus: {
    response: '',
    time: '2016-10-19T10:37:00Z'
  },
  recurrence: null,
  uid: 'iCalUId-value',
  reminderMinutesBeforeStart: 99,
  isOnlineMeeting: true,
  onlineMeetingProvider: 'teamsForBusiness',
  isReminderOn: true,
  hideAttendees: false,
  categories: ['Red category']
};

await client.api('/me/events/{id}')
    .version('beta')
    .update(event);

```