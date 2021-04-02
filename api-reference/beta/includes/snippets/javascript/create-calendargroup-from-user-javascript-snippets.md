---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 94e163ad5af71301e2eae784090cf18817499475
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: 'Personal events'
};

await client.api('/me/calendarGroups')
    .version('beta')
    .post(calendarGroup);

```