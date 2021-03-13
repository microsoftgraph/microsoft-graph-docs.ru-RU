---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 31880b57d458fda3f40572501fe5200aab4afd8f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778189"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rooms = await client.api('/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms')
    .version('beta')
    .get();

```