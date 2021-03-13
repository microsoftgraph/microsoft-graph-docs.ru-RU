---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 89971dbd84df92c9577988f9c011ab963eea68c5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772501"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getrecentnotebooks = await client.api('/me/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)')
    .get();

```