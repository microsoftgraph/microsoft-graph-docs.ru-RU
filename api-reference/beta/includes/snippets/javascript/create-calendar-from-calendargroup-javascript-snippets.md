---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6fae3399d85b0b0069ffd8f36d1637e26ce48994
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: 'Marketing calendar'
};

await client.api('/me/calendargroups/AAMkADYAAAR9NR5AAA=/calendars')
    .version('beta')
    .post(calendar);

```