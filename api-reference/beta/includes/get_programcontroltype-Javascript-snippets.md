---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 749f7edfebb38b0e3ef34df6aa12b0bfdc8aea7f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447112"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/programControlTypes')
    .version('beta')
    .get();

```