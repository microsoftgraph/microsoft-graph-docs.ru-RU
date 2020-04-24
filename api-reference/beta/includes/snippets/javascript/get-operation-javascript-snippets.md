---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c519ddeb979ca7a2d30443bab3126db699f7ec27
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805773"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/authentication/operations/{id}')
    .version('beta')
    .get();

```