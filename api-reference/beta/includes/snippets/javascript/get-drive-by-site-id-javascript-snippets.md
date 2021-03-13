---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fc42b525d3d2f89fbfd21ce58325a00ae594f769
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785842"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/sites/{siteId}/drive')
    .version('beta')
    .get();

```