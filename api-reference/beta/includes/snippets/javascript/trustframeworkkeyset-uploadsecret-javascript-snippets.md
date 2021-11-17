---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6eb5e556f77bb06e8099782d24ca750ccee0237c56e87d9a590f9d2e8c6ded2e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57362695"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKey = {
  use: 'use-value',
  k: 'application-secret-to-be-uploaded',
  nbf: 1508969811,
  exp: 1508973711
};

await client.api('/trustFramework/keySets/{id}/uploadSecret')
    .version('beta')
    .post(trustFrameworkKey);

```