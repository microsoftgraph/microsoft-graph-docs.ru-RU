---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 41ae983a142763fa97a782113746d7a28bd3151f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944808"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let languages = await client.api('/identity/b2cUserFlows/B2C_1_CustomerSignUp/languages')
    .version('beta')
    .get();

```