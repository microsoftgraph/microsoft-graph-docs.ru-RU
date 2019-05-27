---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9bd9468060d310720c588381c312cc9c6d6d39d9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435251"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  accountEnabled: true,
  businessPhones: [
    "businessPhones-value"
  ],
  city: "city-value"
};

let res = await client.api('/me')
    .update({user : user});

```