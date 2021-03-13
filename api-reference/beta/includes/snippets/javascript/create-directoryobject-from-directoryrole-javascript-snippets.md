---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 22bd95221b5f92e5b1424138e38fadb1240c5c2c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808415"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
    '@odata.id':'https://graph.microsoft.com/beta/directoryObjects/2c891f12-928d-4da2-8d83-7d2434a0d8dc'
};

await client.api('/directoryRoles/0afed502-2456-4fd4-988e-3c21924c28a7/members/$ref')
    .version('beta')
    .post(directoryObject);

```