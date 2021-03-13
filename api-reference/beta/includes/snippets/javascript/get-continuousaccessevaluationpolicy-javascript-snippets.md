---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7c3011b5f1c90ed053e8567be3ec0e5a79bd4fbb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809199"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let continuousAccessEvaluationPolicy = await client.api('/identity/continuousAccessEvaluationPolicy')
    .version('beta')
    .get();

```