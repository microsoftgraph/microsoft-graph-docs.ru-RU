---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f74bb9512041406fdb5a6506b24e0d9cd0a39845
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711135"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const refreshSession = {

};

let res = await client.api('/me/drive/items/{id}/workbook/refreshSession')
    .post(refreshSession);

```