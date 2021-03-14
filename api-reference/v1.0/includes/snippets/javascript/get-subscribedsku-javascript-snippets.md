---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 00e4968ea7f722f84cf8a8aedf941cd6cdb04938
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800723"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscribedSku = await client.api('/subscribedSkus/{id}')
    .get();

```