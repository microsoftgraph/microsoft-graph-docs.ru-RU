---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: f1add4a99ec9b1c502cba12c2537881b2fb3dd0d7fb9ee92416ab9c564a90e45
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57053859"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookWorksheet = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}')
    .version('beta')
    .get();

```