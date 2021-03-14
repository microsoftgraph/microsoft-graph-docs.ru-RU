---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3ac03a2e30088c358b3019308d974f3f66f35bfa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793697"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teachers = await client.api('/education/classes/{class-id}/teachers')
    .get();

```