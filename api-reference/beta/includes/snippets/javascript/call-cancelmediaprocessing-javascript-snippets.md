---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: ebf6d327aa8525a39e75abd423a757fb6ede77a3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802928"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancelMediaProcessingOperation = {
  clientContext: 'clientContext-value'
};

await client.api('/communications/calls/{id}/cancelMediaProcessing')
    .version('beta')
    .post(cancelMediaProcessingOperation);

```