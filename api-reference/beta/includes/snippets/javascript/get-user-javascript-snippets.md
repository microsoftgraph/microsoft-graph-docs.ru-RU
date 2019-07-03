---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b576a2f53f1dab69a4518c87a9e41cfcf52085a9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35506060"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me')
    .version('beta')
    .get();

```