---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 3323d3530024c2927aebe8f928796430ffdcca3e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805716"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let patents = await client.api('/me/profile/patents')
    .version('beta')
    .get();

```