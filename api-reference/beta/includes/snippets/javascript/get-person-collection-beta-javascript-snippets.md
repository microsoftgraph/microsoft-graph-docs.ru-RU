---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1e1207b3d2a21ec8093f043dc544ed238ae2b0a3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783071"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let people = await client.api('/me/people')
    .version('beta')
    .get();

```