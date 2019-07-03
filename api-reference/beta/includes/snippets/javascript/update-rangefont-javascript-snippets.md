---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1f609ff13f09d799c5f1baad3103f18133f7111c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35488641"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  bold: true,
  color: "color-value",
  italic: true,
  name: "name-value",
  size: 99,
  underline: "underline-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/font')
    .version('beta')
    .update({workbookRangeFont : workbookRangeFont});

```