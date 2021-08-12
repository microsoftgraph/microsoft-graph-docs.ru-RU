---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 0b803286594fe72890c437034699f908138b62e233321fb66e23f2cc924c2d31
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54237879"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: "#FF0000"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill')
    .update(workbookRangeFill);

```