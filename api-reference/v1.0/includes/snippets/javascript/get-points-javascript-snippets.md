---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 1fc53a8163e1930719a93c96d79d5f382dbbaa46795fcc76dc5bafb5e31b5683
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57307740"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let points = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points')
    .get();

```