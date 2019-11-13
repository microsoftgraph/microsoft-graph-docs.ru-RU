---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: db34c3e42c51a4d39e68b2835a75113846bd233f
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302377"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const answer = {
  callbackUri: "callbackUri-value",
  mediaConfig: {
    @odata.type: "#microsoft.graph.appHostedMediaConfig",
    blob: "<Media Session Configuration Blob>"
  },
  acceptedModalities: [
    "audio"
  ]
};

let res = await client.api('/communications/calls/{id}/answer')
    .version('beta')
    .post(answer);

```