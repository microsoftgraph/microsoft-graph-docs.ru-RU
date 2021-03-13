---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 246b2ec7f9550903aeec50488dd3080969dfba8e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808761"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let content = await client.api('/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content')
    .version('beta')
    .get();

```