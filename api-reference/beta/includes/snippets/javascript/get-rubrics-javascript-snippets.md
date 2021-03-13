---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ef156d0001c7822cd2fec368f92f5c63accb1ceb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rubrics = await client.api('/education/me/rubrics')
    .version('beta')
    .get();

```