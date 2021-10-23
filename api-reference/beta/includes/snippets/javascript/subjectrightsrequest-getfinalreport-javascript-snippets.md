---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cc6c2af80ec15cb91ce31dd5c48465c92d8a187f
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/23/2021
ms.locfileid: "60558991"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/privacy/subjectRightsRequests/{subjectRightsRequestId}/getFinalReport')
    .version('beta')
    .get();

```