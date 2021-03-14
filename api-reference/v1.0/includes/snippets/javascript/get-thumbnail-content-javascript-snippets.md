---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f5fee1db6c70703643cfbefb94f0aa4f1b78aafb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788408"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let content = await client.api('/me/drive/items/{item-id}/thumbnails/{thumb-id}/{size}/content')
    .get();

```