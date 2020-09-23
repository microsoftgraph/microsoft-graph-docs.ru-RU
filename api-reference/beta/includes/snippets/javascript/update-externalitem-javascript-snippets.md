---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f1ee3870aa6e369a3aa16a2f11bd0ab5efa6038c
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48230694"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalItem = {
  acl: [
    {
      type: "everyone",
      value: "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      accessType: "grant",
      identitySource: "azureActiveDirectory"
    }
  ]
};

let res = await client.api('/connections/contosohr/items/TSP228082938')
    .version('beta')
    .update(externalItem);

```