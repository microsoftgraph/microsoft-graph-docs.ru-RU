---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 99d0f2f180ce9ab46c6bb103545029a7b5e374bd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798434"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/directoryRoles/delta')
    .version('beta')
    .get();

```