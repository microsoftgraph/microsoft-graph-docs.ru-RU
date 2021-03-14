---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2997da9f74c667229f87fcf760356c4dbfbf6758
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796904"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contact = await client.api('/me/contacts/{id}')
    .get();

```