---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 66dbac501d9ec8990b9553f2ecbfece2a0861ed4790ca29303ba900f9048935c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57143663"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  index: 3
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/itemAt')
    .post(workbookTableColumn);

```