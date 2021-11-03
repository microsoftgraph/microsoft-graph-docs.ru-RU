---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 31c23feee0821614b63654c5fbfa3353663db6700eef61d565a1cb7ac58c1a12
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57317234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columns = await client.api('/sites/{site-id}/contentTypes/{contentType-id}/columns')
    .version('beta')
    .get();

```