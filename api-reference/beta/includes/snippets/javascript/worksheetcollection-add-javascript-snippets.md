---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 33d617f74f7b519dc85e752b1a6a363b31d95f70
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794250"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookWorksheet = {
  name: 'name-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/add')
    .version('beta')
    .post(workbookWorksheet);

```