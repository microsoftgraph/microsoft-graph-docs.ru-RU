---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fb0bf591b2591a0104e6ceee5b0451e9f1075c5f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471917"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/settings/{id}')
    .version('beta')
    .get();

```