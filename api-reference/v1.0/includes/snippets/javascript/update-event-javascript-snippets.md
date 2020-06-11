---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e6b2584c2e6a10cf0b4e771c0037f6f5fd2b6366
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44680995"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  originalStartTimeZone: "originalStartTimeZone-value",
  originalEndTimeZone: "originalEndTimeZone-value",
  responseStatus: {
    response: "",
    time: "datetime-value"
  },
  recurrence: null,
  iCalUId: "iCalUId-value",
  reminderMinutesBeforeStart: 99,
  isOnlineMeeting: true,
  onlineMeetingProvider: "teamsForBusiness",
  isReminderOn: true,
  categories: ["Red category"]
};

let res = await client.api('/me/events/{id}')
    .update(event);

```