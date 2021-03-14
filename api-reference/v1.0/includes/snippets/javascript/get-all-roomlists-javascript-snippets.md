---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ba1b0c758950a06eec97b97013bd910387d65cb3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809937"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roomlist = await client.api('/places/microsoft.graph.roomlist')
    .get();

```