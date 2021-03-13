---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a4d017815b17f89718af8827361e4f276ef97ce1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810230"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let thumbnails = await client.api('/me/drive/items/{item-id}/thumbnails')
    .version('beta')
    .get();

```