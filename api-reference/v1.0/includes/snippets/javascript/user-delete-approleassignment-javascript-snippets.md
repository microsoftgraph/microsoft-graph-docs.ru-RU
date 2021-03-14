---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a1a3b3c637e1026f22a071ab423aa538ff6efd5e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785652"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{id}/appRoleAssignments/{id}')
    .delete();

```