---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7239521daa99a8f54d5c436de620bd75013fc8fd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785173"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let informationProtectionLabel = await client.api('/me/informationprotection/policy/labels/{id}')
    .version('beta')
    .get();

```