---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 749f7edfebb38b0e3ef34df6aa12b0bfdc8aea7f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35489246"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/programControlTypes')
    .version('beta')
    .get();

```