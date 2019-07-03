---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 241ed1161767c547ef21f543732a59ca7f4144bb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529961"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: "name-value"
};

let res = await client.api('/me/calendarGroups/{id}')
    .version('beta')
    .update({calendarGroup : calendarGroup});

```