---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9d86c65a0187562659ef7f77ae12c8dba0829945
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610163"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const exportPersonalData = {
  storageLocation: "storageLocation-value"
};

let res = await client.api('/users/{id}/exportPersonalData')
    .post(exportPersonalData);

```