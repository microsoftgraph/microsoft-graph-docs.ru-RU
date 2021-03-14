---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9a1767c02ee527f478f866b9d2230975ba24b13f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803425"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directoryRoles = await client.api('/directoryRoles')
    .get();

```