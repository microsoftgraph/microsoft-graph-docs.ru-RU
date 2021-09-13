---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f59eb48b35defcddd2aedb67f77f09f691e54068f1bd1767a1382f8980d39d86
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57211847"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/tokenLifetimePolicies/{id}')
    .delete();

```