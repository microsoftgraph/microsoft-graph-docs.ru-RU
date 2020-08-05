---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d47d0168bbf84d127c553d121a912cf5c7a76994
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566965"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ediscoveryCase = {
    displayName: "My Case 1",
};

let res = await client.api('/compliance/ediscovery/cases')
    .version('beta')
    .post(ediscoveryCase);

```