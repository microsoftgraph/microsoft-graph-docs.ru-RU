---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7460090f6da1d125ac68f4d27f01d204af02e956
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784153"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/todo/lists/AAMkADIyAAAhrbPXAAA=')
    .delete();

```