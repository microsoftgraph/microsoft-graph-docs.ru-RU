---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 560b2ca2235a3dd72ff6828fee1790f99909587f
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341297"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPC = await client.api('/deviceManagement/virtualEndpoint/cloudPCs/9ec90ff8-fd63-4fb9-ab5a-aa4fdcc43ec9')
    .version('beta')
    .get();

```