---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d1c42902976987cc9c23ebc43f99660efab7881f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802367"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let dataPolicyOperation = await client.api('/dataPolicyOperations/{id}')
    .get();

```