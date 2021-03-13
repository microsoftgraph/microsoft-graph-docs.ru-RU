---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 290e3b3e25e4ef39a3cf7faf1471a78cfb2b87a8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794453"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sections = await client.api('/me/onenote/sections')
    .version('beta')
    .get();

```