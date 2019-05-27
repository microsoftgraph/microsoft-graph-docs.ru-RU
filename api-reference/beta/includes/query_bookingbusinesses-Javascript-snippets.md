---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a9b8cae5c796eddb52b507e63199176a2d3845ef
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443035"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/bookingBusinesses')
    .version('beta')
    .get();

```