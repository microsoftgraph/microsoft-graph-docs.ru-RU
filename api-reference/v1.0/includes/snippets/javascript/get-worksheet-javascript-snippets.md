---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 2888e29cc367ccc66b76379f743ff8c3f3b30cdc1e441659d4091b29f33eb477
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57210644"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookWorksheet = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}')
    .get();

```