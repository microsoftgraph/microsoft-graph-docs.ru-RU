---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ab01fb3b27b1962eba1120b4a0bf76906876845f
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638503"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  subject: "subject-value",
  body: {
    contentType: "",
    content: "content-value"
  },
  inferenceClassification: "other"
};

let res = await client.api('/me/messages/{id}')
    .update(message);

```