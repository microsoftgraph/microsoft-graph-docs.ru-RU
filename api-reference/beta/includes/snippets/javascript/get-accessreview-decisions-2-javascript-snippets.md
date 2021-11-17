---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 6856d2ab6ec9cc29d0bd6892fb341a01e4aeccec51f04ea4a0043563e6b3ae49
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57051206"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let myDecisions = await client.api('/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/myDecisions')
    .version('beta')
    .get();

```