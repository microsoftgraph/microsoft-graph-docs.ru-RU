---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 508172f4bf6ff1c3912973969dcc8057dbf3d93d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798489"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/groups/{groupId}/drives')
    .version('beta')
    .get();

```