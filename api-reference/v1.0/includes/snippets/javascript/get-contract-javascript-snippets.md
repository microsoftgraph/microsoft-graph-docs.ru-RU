---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: bb9b5e129214015b0b2a1b5f0aae5149aac1b4f2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780381"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contract = await client.api('/contracts/{id}')
    .get();

```