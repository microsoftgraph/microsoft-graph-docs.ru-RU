---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: d7e9821f01cf21e930bb664cd00d9588aa48b156a54b96e84c75a0f6f1578317
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57248653"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookTableSort = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort')
    .version('beta')
    .get();

```