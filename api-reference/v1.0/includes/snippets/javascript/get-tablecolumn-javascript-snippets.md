---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 75e088b63249dd15420cd98f893c4768183c04f986bde52d99ed41d55e67c45e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57195740"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookTableColumn = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}')
    .get();

```