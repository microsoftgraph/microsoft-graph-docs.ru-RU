---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: fe00437b93c609652d90edc8e724223b61dfc011
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793791"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationClass = await client.api('/education/classes/11023')
    .version('beta')
    .get();

```