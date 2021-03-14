---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 5adc986f43b86b1d2f2524700c63d748c7b1fd0f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803594"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  bold: true,
  color: '#4B180E',
  size: 26
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format/font')
    .update(workbookRangeFont);

```