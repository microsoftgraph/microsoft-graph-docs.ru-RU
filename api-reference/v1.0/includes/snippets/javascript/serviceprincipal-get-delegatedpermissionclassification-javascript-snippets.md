---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 01dd51f9de837e22da86deba88049b66c9ddfb36
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786826"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delegatedPermissionClassifications = await client.api('/servicePrincipals/{id}/delegatedPermissionClassifications')
    .get();

```