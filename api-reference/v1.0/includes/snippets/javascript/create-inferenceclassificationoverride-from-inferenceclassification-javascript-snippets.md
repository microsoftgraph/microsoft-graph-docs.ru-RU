---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d798b35230a6a3968a986c232bc092ecede56619
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "36638514"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const inferenceClassificationOverride = {
  classifyAs: "focused",
  senderEmailAddress: {
    name: "Samantha Booth",
    address: "samanthab@adatum.onmicrosoft.com"
  }
};

let res = await client.api('/me/inferenceClassification/overrides')
    .post(inferenceClassificationOverride);

```