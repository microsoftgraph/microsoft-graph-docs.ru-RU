---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: e627527dc1d64b99886167e5652d67c5a94a9870
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785262"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let personAnnualEvent = await client.api('/me/profile/anniversaries/{id}')
    .version('beta')
    .get();

```