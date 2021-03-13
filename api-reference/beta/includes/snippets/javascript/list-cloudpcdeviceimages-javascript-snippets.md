---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0642a74a6908510e686f4ace36620402785fdd9a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805901"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let deviceImages = await client.api('/deviceManagement/virtualEndpoint/deviceImages')
    .version('beta')
    .get();

```