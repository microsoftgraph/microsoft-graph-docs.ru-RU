---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cb4a01e5a0dd80762021b77bf21669628ff124d0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784807"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let itemPhone = await client.api('/me/profile/phones/{id}')
    .version('beta')
    .get();

```