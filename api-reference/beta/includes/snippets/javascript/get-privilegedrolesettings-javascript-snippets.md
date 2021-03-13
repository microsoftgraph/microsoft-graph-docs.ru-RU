---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bd7be266ca6eff8cb8d43fd153e3a9e43b2eb5a2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785043"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRoleSettings = await client.api('/privilegedRoles/{id}/settings')
    .version('beta')
    .get();

```