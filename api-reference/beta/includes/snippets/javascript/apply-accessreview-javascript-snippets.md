---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4319b3c180228904f0b942f03f824bcdca027bbd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/applyDecisions')
    .version('beta')
    .post();

```