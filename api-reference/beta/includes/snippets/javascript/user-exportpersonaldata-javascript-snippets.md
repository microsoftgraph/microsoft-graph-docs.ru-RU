---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2d861ad9fcb91c5527c6d1f3235e630e75a0f78a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const exportPersonalData = {
  storageLocation: 'storageLocation-value'
};

await client.api('/users/{id}/exportPersonalData')
    .version('beta')
    .post(exportPersonalData);

```