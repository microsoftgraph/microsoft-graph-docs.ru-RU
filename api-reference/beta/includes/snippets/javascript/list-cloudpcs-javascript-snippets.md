---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7fcc3b3e5ab71521f88dde4a01d839abfa28a1c6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785853"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPCs = await client.api('/deviceManagement/virtualEndpoint/cloudPCs')
    .version('beta')
    .get();

```