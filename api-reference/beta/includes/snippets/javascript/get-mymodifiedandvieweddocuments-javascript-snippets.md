---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5faf726d86e2ea6d42109248deddd22a0c06b5a7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779862"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let used = await client.api('/me/insights/used')
    .version('beta')
    .orderby('LastUsed/LastAccessedDateTime desc')
    .get();

```