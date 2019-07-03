---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 377dcfdd761bc1947e28f63dc10c2d113a06a3eb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529198"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const refreshSession = {

};

let res = await client.api('/me/drive/items/{id}/workbook/refreshSession')
    .version('beta')
    .post(refreshSession);

```