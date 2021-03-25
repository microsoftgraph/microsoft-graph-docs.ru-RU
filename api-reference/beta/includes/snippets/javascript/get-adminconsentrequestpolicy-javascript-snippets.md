---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 210f4bcb27a065b79870fb41e174e6fc38c1a0ce
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201502"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let adminConsentRequestPolicy = await client.api('/policies/adminConsentRequestPolicy')
    .version('beta')
    .get();

```