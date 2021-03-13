---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: caffa900baa1a5130a1d41d9230118b11ddfd437
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790383"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeOffReason = {
  displayName: 'Vacation',
  iconType: 'plane',
  isActive: true
};

await client.api('/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}')
    .version('beta')
    .put(timeOffReason);

```