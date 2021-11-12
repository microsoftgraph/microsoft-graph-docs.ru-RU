---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: c34ae1a642e8bfc54f55537a8ec4dca321c592ec578f1bf5301496a47d97ff4f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57053043"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rows = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows')
    .version('beta')
    .get();

```