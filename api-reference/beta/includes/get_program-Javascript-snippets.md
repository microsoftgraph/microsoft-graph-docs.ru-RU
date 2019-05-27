---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7b99c3dff2098cae61f03ffefe988bfa660cc84b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/programs')
    .version('beta')
    .get();

```