---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 93832f79006af6e8737b990401871f6a246775c5
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591721"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/tokenIssuancepolicies/{id}')
    .version('beta')
    .get();

```