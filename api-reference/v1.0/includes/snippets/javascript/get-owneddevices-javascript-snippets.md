---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 35244244ecbed190c7b5f61007ebbec8a49d0f03
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802959"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let ownedDevices = await client.api('/me/ownedDevices')
    .get();

```