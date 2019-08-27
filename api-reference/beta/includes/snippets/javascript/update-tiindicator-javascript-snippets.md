---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9e94bf09f6c9006b70ae6204f84d6e523d344185
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638302"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tiIndicator = {
  additionalInformation: "additionalInformation-after-update",
  confidence: 42,
  description: "description-after-update",
};

let res = await client.api('/security/tiIndicators/{id}')
    .version('beta')
    .update(tiIndicator);

```