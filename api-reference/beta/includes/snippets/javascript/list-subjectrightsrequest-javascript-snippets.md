---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 81bed5c55a6e5c8a021f798a547f1be9af47e4cb
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561649"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subjectRightsRequests = await client.api('/privacy/subjectRightsRequests')
    .version('beta')
    .get();

```