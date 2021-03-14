---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 25e0f6b8927a8f5242745d4418ed24ebdb0fe258
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780872"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let users = await client.api('/users')
    .get();

```