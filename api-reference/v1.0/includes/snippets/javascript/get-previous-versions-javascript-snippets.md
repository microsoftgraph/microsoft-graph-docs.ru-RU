---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c87d8c22bbd760fc567dbbc5a594304b37a9a5d1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798641"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let versions = await client.api('/me/drive/items/{item-id}/versions')
    .get();

```