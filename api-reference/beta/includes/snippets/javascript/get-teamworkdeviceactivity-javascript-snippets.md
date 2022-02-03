---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6a021e283e8724a5fe6adfa0be95065d46c0856d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347449"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let teamworkDeviceActivity = await client.api('/teamwork/devices/1ae3fe60-fe60-1ae3-60fe-e31a60fee31a/activity')
    .version('beta')
    .get();

```