---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0b291a454ef1ccba3bf2ba81549efa2dd99aa1c5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800393"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/security/securityActions/{id}/cancelSecurityAction')
    .version('beta')
    .post();

```