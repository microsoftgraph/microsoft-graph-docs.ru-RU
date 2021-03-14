---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 03d8d7089983c30bd648826d8a1c53460e5ffa99
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787197"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: 'name-value',
  classId: 'classId-value',
  changeKey: 'changeKey-value'
};

await client.api('/me/calendarGroups')
    .post(calendarGroup);

```