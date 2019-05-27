---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5ea2a96f99eb2a9f1f4355d40d45ae5dc19410d8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444218"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/riskyUsers')
    .version('beta')
    .get();

```