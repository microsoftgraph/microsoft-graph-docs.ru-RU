---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1ac715fb6709031671f7eb31c836cce231aecea6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438576"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/settings/{id}')
    .version('beta')
    .delete();

```