---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6e08ebe113c02f5b7b2fda948eb4d8c66e53361d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446853"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}/registeredOwners')
    .version('beta')
    .get();

```