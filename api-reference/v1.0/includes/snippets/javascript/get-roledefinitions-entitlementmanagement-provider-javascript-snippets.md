---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 605e6d22e2bd5d88c54691f280e09ff13609595d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207155"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleDefinitions = await client.api('/roleManagement/entitlementManagement/roleDefinitions')
    .get();

```