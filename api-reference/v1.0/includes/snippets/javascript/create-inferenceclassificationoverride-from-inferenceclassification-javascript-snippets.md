---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ae050757916f435ad7a7ff98675ff4183f2436d4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780032"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const inferenceClassificationOverride = {
  classifyAs: 'focused',
  senderEmailAddress: {
    name: 'Samantha Booth',
    address: 'samanthab@adatum.onmicrosoft.com'
  }
};

await client.api('/me/inferenceClassification/overrides')
    .post(inferenceClassificationOverride);

```