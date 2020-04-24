---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 36394eaceaf2f6a6a4b895c0f1424a1b44a8ff3c
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806214"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/oauth2permissiongrants/delta')
    .version('beta')
    .get();

```