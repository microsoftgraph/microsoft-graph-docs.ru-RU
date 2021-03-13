---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b2d84583fccd770d5f4388dcecdc6727d2cfd2d6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780186"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let taskDefinitions = await client.api('/print/taskDefinitions')
    .version('beta')
    .get();

```