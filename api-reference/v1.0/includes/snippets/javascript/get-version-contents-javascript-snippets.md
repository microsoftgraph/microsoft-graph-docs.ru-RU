---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 63e2642f453eaf2d52ece123168cdefd5b932061
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802287"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/me/drive/items/{item-id}/versions/{version-id}/content')
    .get();

```