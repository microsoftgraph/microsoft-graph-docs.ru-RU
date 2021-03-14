---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: dff6ef0467761408a02fd441bd9ba4e44f2f5afe
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804871"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissionGrantPolicy = await client.api('/policies/permissionGrantPolicies/microsoft-user-default-low')
    .get();

```