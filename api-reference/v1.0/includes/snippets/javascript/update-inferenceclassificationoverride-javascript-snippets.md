---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d8c0d3a7368f920892af4776b0a5a31e4766e9c0
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638513"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const inferenceClassificationOverride = {
  classifyAs: "focused"
};

let res = await client.api('/me/inferenceClassification/overrides/{id}')
    .update(inferenceClassificationOverride);

```