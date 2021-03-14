---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 72575b691455ef1816f359337e8dc136d7bf7d4b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786531"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let worksheets = await client.api('/me/drive/items/{id}/workbook/worksheets')
    .get();

```