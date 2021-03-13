---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 26f541ab1910f9e1bbf294aeae22f4d4dd6c8c5c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800348"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let outcomes = await client.api('/education/me/assignments/{id}/submissions/{id}/outcomes')
    .version('beta')
    .get();

```