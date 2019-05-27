---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 077985459879a065e7df6d3dc05faec33d08a8a6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447266"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoles/{id}/summary')
    .version('beta')
    .get();

```