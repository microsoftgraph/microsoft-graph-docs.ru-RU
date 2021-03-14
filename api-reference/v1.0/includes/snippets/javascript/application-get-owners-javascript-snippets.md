---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f90772907fde6f3ec72231f8e5b9b0f79bf1819e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806972"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let owners = await client.api('/applications/{id}/owners')
    .get();

```