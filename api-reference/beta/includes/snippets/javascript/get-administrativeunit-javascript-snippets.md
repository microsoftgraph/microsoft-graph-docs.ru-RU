---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: a6c94f55e992bb6dc2774efe209f84b774da033070ee5013312d5cf882d965ed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57050894"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let administrativeUnit = await client.api('/administrativeUnits/{id}')
    .version('beta')
    .get();

```