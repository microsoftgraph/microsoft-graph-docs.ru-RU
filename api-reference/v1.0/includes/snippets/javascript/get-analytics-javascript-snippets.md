---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2cd1c84b6c92764d0561100704926b23f2d2e835
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801427"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemAnalytics = await client.api('/drives/{drive-id}/items/{item-id}/analytics')
    .get();

```