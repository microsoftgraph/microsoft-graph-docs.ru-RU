---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c38efeeb213dd6d4ef30327e96ccd4a80e90676a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810224"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: 'name-value'
};

await client.api('/me/calendarGroups/{id}')
    .version('beta')
    .update(calendarGroup);

```