---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a760fa14e297d9373067de7ac6e5fc5d17eb2f75
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780916"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcOnPremisesConnection = await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections/{id}')
    .version('beta')
    .get();

```