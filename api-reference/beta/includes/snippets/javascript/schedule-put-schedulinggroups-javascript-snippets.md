---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 34634eced3b113dda15202e945cad5fc0d526087373e0794e956177614b1d0ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57364674"
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

await client.api('/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}')
    .version('beta')
    .put(schedulingGroup);

```