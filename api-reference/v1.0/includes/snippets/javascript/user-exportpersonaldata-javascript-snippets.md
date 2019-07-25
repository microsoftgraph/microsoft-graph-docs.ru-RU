---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 9d86c65a0187562659ef7f77ae12c8dba0829945
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715045"
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