---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7f2bd0b81beb2c8f4bdd94b7563e45517868e236
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785212"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let versions = await client.api('/me/drive/items/{item-id}/versions')
    .version('beta')
    .get();

```