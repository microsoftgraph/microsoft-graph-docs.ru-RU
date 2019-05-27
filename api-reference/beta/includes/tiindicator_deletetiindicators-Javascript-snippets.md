---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f69cfc9636fe5e6c977b293576501aacf7f2ee07
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34469316"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ResultInfo = {
  value: [
    "id-value1",
    "id-value2"
  ]
};

let res = await client.api('/security/tiIndicators/deleteTiIndicators')
    .version('beta')
    .post(ResultInfo);

```