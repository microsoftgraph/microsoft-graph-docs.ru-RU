---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a4d42f15400c9f978948a1db6ad783f25726083d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798683"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let publications = await client.api('/me/profile/publications')
    .version('beta')
    .get();

```