---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f97bd015d7aec7aa59c6ec733a9c3ea8bf925cf5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793910"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schedulingGroup = {
  displayName: 'Cashiers',
  isActive: true,
  userIds: [
    'c5d0c76b-80c4-481c-be50-923cd8d680a1',
    '2a4296b3-a28a-44ba-bc66-0274b9b95851'
  ]
};

await client.api('/teams/{teamId}/schedule/schedulingGroups')
    .version('beta')
    .post(schedulingGroup);

```