---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 7f2222f025fb4e43940609d542ff0369a8f38f04e61c8f52932f43df25a7ebe6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57141889"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMemberOf = await client.api('/devices/{id}/transitiveMemberOf')
    .get();

```