---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: b32a87d85c4b35651c175ed06713221d1a3bc972
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446276"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/securityActions')
    .version('beta')
    .get();

```