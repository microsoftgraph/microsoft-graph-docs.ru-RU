---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4accd33262b044837928ecfbb9492eb79ad1fa37
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35487864"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/tiIndicators/{id}')
    .version('beta')
    .delete();

```