---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d4d633794f49dbc98f2d49627eb4256fcaa8a5b6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807752"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drives = await client.api('/me/drives')
    .get();

```