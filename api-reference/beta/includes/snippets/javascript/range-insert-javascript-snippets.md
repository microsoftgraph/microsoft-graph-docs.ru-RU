---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4dd6648b0b157f33a707dd0f99c7a9faf32ead57
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35529858"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRange = {
  shift: "shift-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/insert')
    .version('beta')
    .post(workbookRange);

```