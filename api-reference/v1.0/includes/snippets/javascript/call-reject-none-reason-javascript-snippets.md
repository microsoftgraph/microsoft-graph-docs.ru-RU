---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a8ef720f5780e1d764f8374ff8c6723a5fd7108cf47fa212260266d041713ed2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57318010"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reject = {
  reason: 'none'
};

await client.api('/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896/reject')
    .post(reject);

```