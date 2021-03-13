---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d646941ccd040993347497239aed718484169652
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796105"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalConnection = {
  id: 'contosohr',
  name: 'Contoso HR',
  description: 'Connection to index Contoso HR system'
};

await client.api('/external/connections')
    .version('beta')
    .post(externalConnection);

```