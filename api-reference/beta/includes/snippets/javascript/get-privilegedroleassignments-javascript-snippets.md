---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fc42c2d690681f4e3b9098380b770dabaca1ec60
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794603"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRoleAssignments = await client.api('/privilegedRoleAssignments')
    .version('beta')
    .filter('isElevated eq true and expirationDateTime ne null or isElevated eq false')
    .get();

```