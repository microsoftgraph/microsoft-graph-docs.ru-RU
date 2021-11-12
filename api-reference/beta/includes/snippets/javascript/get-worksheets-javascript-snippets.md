---
description: Автоматически созданный файл. НЕ ИЗМЕНЯТЬ
ms.openlocfilehash: 4421eeeed821384bcf535b6c091773f75fe00e9514ac25f2b69bf4aa1f5737fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "57142257"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let worksheets = await client.api('/me/drive/items/{id}/workbook/worksheets')
    .version('beta')
    .get();

```