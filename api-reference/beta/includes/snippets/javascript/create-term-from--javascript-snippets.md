---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4c902b7620368fafbd923446d53bb7a988d1d6bd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799977"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const term = {
  labels: [
    {
      languageTag: 'en-US',
      name: 'Car',
      isDefault: true
    }
  ]
};

await client.api('/termStore/sets/{setId}/terms')
    .version('beta')
    .post(term);

```