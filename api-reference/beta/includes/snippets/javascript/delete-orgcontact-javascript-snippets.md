---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 163ba5e8f80aaabbe2d40ecca78ed4cc723a4180
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808496"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/contacts/{id}')
    .version('beta')
    .delete();

```