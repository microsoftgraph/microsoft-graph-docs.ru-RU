---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9cc431cc6cfe760089784b71fad86dd769129c6a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788070"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let personWebsite = await client.api('/me/profile/websites/{id}')
    .version('beta')
    .get();

```