---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: cf748c2ea03a62c15a0de3730a7c785cd08dba60b15657c9fb718953229cd5aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57052746"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let awards = await client.api('/me/profile/awards')
    .version('beta')
    .get();

```