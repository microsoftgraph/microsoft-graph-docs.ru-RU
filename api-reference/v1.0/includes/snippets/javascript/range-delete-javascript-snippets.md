---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 98ccd23fe09f9a604409147102fdec63ca87f2fd600c24912b67d0a418d765bd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57254781"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _delete = {
  shift: 'shift-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/delete')
    .post(_delete);

```