---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e60fc327c077c0ed40c4109f813e136499d1bff5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784192"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let lists = await client.api('/me/todo/lists')
    .version('beta')
    .get();

```