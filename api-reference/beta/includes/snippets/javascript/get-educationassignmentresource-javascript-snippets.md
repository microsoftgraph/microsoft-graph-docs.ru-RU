---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7373a89b8117f17e2f3e0da195b85843a1229218
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781856"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationAssignmentResource = await client.api('/education/classes/11021/assignments/19002/resources/22002')
    .version('beta')
    .get();

```